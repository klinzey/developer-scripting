## The Marionette Node Parametric Object

The Marionette Node is implemented by a piece of Python code. When executing the Marionette Network, Vectorworks traverses the connections between the nodes and builds up a composite Python script from the code of each node.

The code for each node can be accessed through the 'Edit...' button on the node object info palette - shape pane.

Before proceeding with this article, make sure you familiarize yourself with the [Marionette Basics](Basics.md) first.

Also, knowledge of [Python](../../Python/README.md) is required for the reader of this article. See [Python#How to start with Python](../../Python/README.md#how-to-start-with-python).

## Define The Node

The addition node has two input ports and one output port;

![A simple Marionette node to add two numbers](files/MarionetteNodeAdd.png)

The code for this node (available via the Edit button on the Object Info Palette - Shape Pane (OIP) when the node is selected) is:
```py
@Marionette.NodeDefinition
class Params(metaclass = Marionette.OrderedClass):
	this = Marionette.Node( 'Add' )
	a = Marionette.PortIn( 0 )
	b = Marionette.PortIn( 0 )
	out = Marionette.PortOut()
	k = Marionette.OIPControl( 'Multiplier', Marionette.WidgetType.Real, 1 )
	
def RunNode(self):
	sum = self.Params.a.value + self.Params.b.value
	self.Params.out.value = sum * self.Params.k.value
```

The code of the Marionette Node is composed of two pieces:
* Params -- a class Params that defines the node, the input and output parameters, and the OIPControl widgets displayed on the OIP when the node is selected.
* RunNode -- a function that is executed (several times or once, depending on the data mixing) as part of the network execution.

### Params: The Node Definition

```py
this = Marionette.Node( 'Add' )
```

The `Marionette.Node` class defines the Node by providing the following information as parameters:
* typeName -- this is the type name of the node used to display on the drawing.
  * This name is recommended to be in English.
  * If the name needs to be displayed in a different language see [Localizing a Node](#localizing-a-node) below.

### Params: Input Ports

```py
a = Marionette.PortIn( 0 )
```

Each input port is a variable of type Marionette.PortIn class. The default value of the port is any of the built-in types in Python: https://docs.python.org/3/library/stdtypes.html

The input port is created with a default value as parameter. This port variable will be initialized to this value if the node is executed without the port being connected to an output port.

The variable name will be used as a text for the node's port on the drawing. If you need to customize that, or if you need to provide it in another language, see [Localizing a Node](#localizing-a-node) below.

### Params: Output Ports

```py
a = Marionette.PortOut()
```

Each input port is a variable of type Marionette.PortOut class.

The variable name will be used as a text for the node's port on the drawing. If you need to customize that, or if you need to provide it in another language, see [Localizing a Node](#localizing-a-node) below.

### RunNode: Execution

```py
def RunNode(self):
	sum = self.Params.a.value + self.Params.b.value
	self.Params.out.value = sum
```

When the node is being executed as part of a network, Vectorworks will initialize the values of the input ports and run the code inside the 'RunNode' function. The main idea of this function is to get the values from the input ports, and produce values in the output ports.

If this node needs to be repeated, the function `RunNode` will be executed for each repeat and Vectorworks will make sure the input ports are with the correct values for each iteration as described in [Mixing Data Flow](Basics.md#mixing-data-flow).

The ports' values can be accessed by using the port variable name, as defined in the Params class:
```py
self.Params.<varName>.value
```

This code contains the logic of the node, and it might use any built-in python functions, and or the APIs provided by Python Scripting. You can refer to the [Function Reference](../../Function%20Reference/README.md) for a list of available calls.

### Object Info Palette - Shape Pane

Along with the input and output ports, each node can define OIP (Object Info Palette) control widgets when the node object in the drawing is selected:

```py
k = Marionette.OIPControl( 'Multiplier', Marionette.WidgetType.Real, 1)
```

A variable is defined to receive the value of the OIP control.

The parameters of the Marionette.OIPControl are defined as:
* text -- defines the text that appears on the left of the control widget that will be displayed on the OIP
  * If you need to provide it in another language, see [Localizing a Node](#localizing-a-node) below.
* type -- the type of the widget. See below for a list of available types
* default value -- the initial value of the widget

Here is an example of a node with all available OIP control widgets:

![Marionette OIP](files/MarionetteOIP.png)

The available widgets and their corresponding types are:
* Integer -- an integer value
```py
p0 = Marionette.OIPControl( 'Integer', Marionette.WidgetType.Int, 1)
```

* Boolean -- a checked/unchecked value
```py
p1 = Marionette.OIPControl( 'Boolean', Marionette.WidgetType.Bool, True)
```

* Real -- a real value
```py
p2 = Marionette.OIPControl( 'Real', Marionette.WidgetType.Real, 3.14)
```

* Dimension -- a linear dimension value in the units of the current document
```py
p3 = Marionette.OIPControl( 'Dimension', Marionette.WidgetType.RealCoord, 3.14)
```

* Angle -- an angular value in the units of the current document
```py
p4 = Marionette.OIPControl( 'Angle', Marionette.WidgetType.RealAngle, 3.14)
```

* Area -- an area value in the units of the current document
```py
p5 = Marionette.OIPControl( 'Area', Marionette.WidgetType.RealArea, 3.14)
```

* Volume -- a volume value in the units of the current document
```py
p6 = Marionette.OIPControl( 'Volume', Marionette.WidgetType.RealVolume, 3.14)
```

* Test -- a text value
```py
p7 = Marionette.OIPControl( 'Text', Marionette.WidgetType.Text, 'Text')
```

* Static Information -- a text displayed as a single line*
```py
p8 = Marionette.OIPControl( 'Static Information', Marionette.WidgetType.TextStatic, 'Text')
```

* Static Value -- a text displayed as named parameter value
```py
p9 = Marionette.OIPControl( 'Static Value', Marionette.WidgetType.TextStaticParam, 'Text')
```

* Popup -- a text choice popup
```py
p10 = Marionette.OIPControl( 'Popup', Marionette.WidgetType.Popup, 0, ['choice 1', 'choice 2'])
```

* Class -- a class choice popup
```py
p11 = Marionette.OIPControl( 'Class', Marionette.WidgetType.PopupClasses, 'None')
```

* Layer -- a layer choice popup
```py
p12 = Marionette.OIPControl( 'Layer', Marionette.WidgetType.PopupLayers, 'Design Layer-1')
```

* Separator -- this control is used to visually separate different groups of parameters. It has no control behavior for the user
```py
p13 = Marionette.OIPControl( 'Separator', Marionette.WidgetType.Separator, 'Separator Text')
```

* PopupTextures -- a texture choice popup
```py
p14 = Marionette.OIPControl('Texture', Marionette.WidgetType.PopupTextures, 0)
```

* Button -- a button
```py
p15 = Marionette.OIPControl( 'Button', Marionette.WidgetType.Button, 'script', 'description')
```

* Slider -- a slider control that can be defined by the user
```py
p16 = Marionette.OIPControl( 'Integer', Marionette.WidgetType.Slider, 0, 'description', 0, 25)
```

* Radio Button -- a radio button that may have choices defined by the user
```py
p17 = Marionette.OIPControl( 'Radio Button', Marionette.WidgetType.RadioButton, 0, ['choice 1', 'choice 2'])
```

## Node Description

Each node can define a description text that will help the user understand what the node does and what does the input and output parameters mean.

The description is provided by calling the `this.SetDescription` function with the text of the description.

Note: You can use '\n' symbol to define a multi-line description.
  * Also, for the sake of pretty code, you can split the text into several lines.
  * If the description text needs to be in a different language see [Localizing a Node](#localizing-a-node) below.

```py
@Marionette.NodeDefinition
class Params(metaclass = Marionette.OrderedClass):
	this = Marionette.Node( 'Add' )
	this.SetDescription( 'This node will add the two numbers from the input ports and produce a the sum in the result port\n'
				'Port a : input value for the sum\n'
				'Port b : input value for the sum\n'
				'Port out : output sum of the input ports' )

	a = Marionette.PortIn( 0 )
	b = Marionette.PortIn( 0 )
	out = Marionette.PortOut()
	
def RunNode(self):
	sum = self.Params.a.value + self.Params.b.value
	self.Params.out.value = sum
```

# Absorbing List Inputs

A node might be defined not to be repeated when a list of data is presented in any of the inputs. By default, nodes are repeated in this case as defined in [Marionette Basics#Data Flow](Basics.md#data-flow).

When a node is to be executed only once [Marionette Basics#Absorbing Data Flow](Basics.md#absorbing-data-flow), Vectorworks will let the execution script of the node recognize and handle the input data as is (single value or list). Then the output could be produced as a single value or list as well.

To make a node absorb list inputs and be repeated only once, you must call `SetListAbsorb` on the Marionette.Node variable in the node definition section.

Here is an example of a sum node, that will sum up all input values from a single port and output a single value.

```python
@Marionette.NodeDefinition
class Params(metaclass=Marionette.OrderedClass):
    this = Marionette.Node('Sum')
    this.SetListAbsorb()              # mark this node as list absorbing
    data = Marionette.PortIn([])      # almost always the input defaults should be empty list
    out = Marionette.PortOut()

def RunNode(self):
    result = 0
    try:
        for v in self.Params.data.value:
            result = result + v
    except:
        result = self.Params.data.value

    self.Params.out.value = result
```

The example makes sure to try-catch for the cases when the input value is not an iterable value. There are different ways to check for a list of data in Python, and the developer of the node should choose the most appropriate for the case.

Note that if the node has several inputs, the inputs must be manually mixed to produce the output. The easiest way is to use `zip` or `itertools.zip_longest`:

```python
@Marionette.NodeDefinition
class Params(metaclass=Marionette.OrderedClass):
    this = Marionette.Node('Sum')
    this.SetListAbsorb()              # mark this node as list absorbing
    a = Marionette.PortIn([])         # almost always the input defaults should be empty list
    b = Marionette.PortIn([])         # almost always the input defaults should be empty list
    out = Marionette.PortOut()

def RunNode(self):
    result = 0
    try:
        list1 = self.Params.a.value
        list2 = self.Params.b.value
        for a, b in zip(list1, list2):
            result = result + a + b
    except:
        result = self.Params.data.value

    self.Params.out.value = result
```

# Localizing a Node

There are two methods of providing localization for the nodes. However, third-party developers would be most interested in the first method as it will allow providing custom resources with the localized strings. The default content provided with Vectorworks uses the automated method.

## Custom Localization

Here is an example of a fully localized node:

```python
@Marionette.NodeDefinition
class Params(metaclass=Marionette.OrderedClass):
    this = Marionette.Node('Add', 'Localized Node Name')
    this.SetDescription('localized description')
    a = Marionette.PortIn(0, 'localized port a')
    b = Marionette.PortIn(0, 'localized port b')
    out = Marionette.PortOut('localized port out')
    k = Marionette.OIPControl('localized OIP name', Marionette.WidgetType.Real, 1)

def RunNode(self):
    sum = self.Params.a.value + self.Params.b.value
    self.Params.out.value = sum * self.Params.k.value
```

The localized strings for the different components are provided as an extra parameter, or just the string contains the localized text:

* **Definition** -- additional, and optional parameter provides the localized name of the node to be used on the drawing.
* **Description** -- the `SetDescription` call accepts the description text, which is provided as is.
* **Ports** -- each of the ports (input and output) have an additional, and optional parameter to provide the localized name of the port to be used on the drawing.
* **OIPControl** -- each control variable is defined with text, which is used as provided.

Actually, using fixed strings in code is not recommended as it restricts the use of the node in only one language.

Vectorworks has a resource system that is designed to provide localized strings from a resource path and a string key. The resource system is based on VWR files that contain vwstring, UTF-16 encoded text files to provide localized strings.

A node implementation can use the Python Script function [GetVWRString](../../Function%20Reference/Functions/GetVWRString.md) to obtain the localized string.

So, instead of fixing the strings in the Python code, you can use the script function to get the string:

```python
@Marionette.NodeDefinition
class Params(metaclass=Marionette.OrderedClass):
    this = Marionette.Node('Add', vsGetVWRString('CustomResource/Strings/MyResource', 'Add'))
    this.SetDescription(vsGetVWRString('CustomResource/Strings/MyResource', 'Add.Description'))
    a = Marionette.PortIn(0, vsGetVWRString('CustomResource/Strings/MyResource', 'Add.PortIn.a'))
    b = Marionette.PortIn(0, vsGetVWRString('CustomResource/Strings/MyResource', 'Add.PortIn.b'))
    out = Marionette.PortOut(vsGetVWRString('CustomResource/Strings/MyResource', 'Add.PortOut.out'))
    k = Marionette.OIPControl(vsGetVWRString('CustomResource/Strings/MyResource', 'Add.OIP.Multiplier'), Marionette.WidgetType.Real, 1)

def RunNode(self):
    sum = self.Params.a.value + self.Params.b.value
    self.Params.out.value = sum
```

Then the MyResource.vwstrings file in the 'CustomResource.vwr' resource file would look like this:

```r
"Add" = "Localized Node Name";
"Add.Description" = "localized description";
"Add.PortIn.a" = "localized port a";
"Add.PortIn.b" = "localized port b";
"Add.PortOut.out" = "localized port out";
"Add.OIP.Multiplier" = "localized OIP name";
```

The string keys in this example are built up with the naming standard used by the automated localization system. However, the developer for the node might decide to use a different naming standard as the relation between code and resources is determined by the code of the node itself.

## Automatic Localization

The automatic localization system is designed to work for the nodes provided in the default content of Vectorworks. It is not recommended for third-party developers to modify the resources of Vectorworks as there is no way to ensure that those resources will be preserved when updating or upgrading the software.

This information is provided as a reference, and a typical third-party developer should use the Custom Localization described above to provide localization of the custom nodes.

For a node that doesn't provide any localized strings in the optional parameters, the localized strings will automatically be looked up in the Marionette.vwr resource file, and used if they exist.

For example, the node:

```python
@Marionette.NodeDefinition
class Params(metaclass=Marionette.OrderedClass):
    this = Marionette.Node('Add')
    a = Marionette.PortIn(0)
    b = Marionette.PortIn(0)
    out = Marionette.PortOut()
    k = Marionette.OIPControl('Multiplier', Marionette.WidgetType.Real, 1)
    p10 = Marionette.OIPControl('Popup', Marionette.WidgetType.Popup, 0, ['choice 1', 'choice 2'])

def RunNode(self):
    sum = self.Params.a.value + self.Params.b.value
    self.Params.out.value = sum * self.Params.k.value
```

Vectorworks will automatically try to load the localized strings for the node name, port names, and OIP control from the `LocalizedNodeStrings.vwstrings` file in the Strings of Marionette.vwr resource file.

This automatic look-up will build up a key from the corresponding node name, port name, or fixed string:
* **Node name** -- the string key will be: "<node name>"
* **Node description** -- the string key will be: "<node name>.Description"
* **Input port name** -- the string key will be: "<node name>.PortIn.<port name>"
* **Output port name** -- the string key will be: "<node name>.PortOut.<port name>"
* **OIP Control** -- the string key will be: "<node name>.OIP.<text>"

As an example, the corresponding entries in `LocalizedNodeStrings.vwstrings` for the example above will be:

```r
"Add" = "Localized Node Name";
"Add.Description" = "localized description";
"Add.PortIn.a" = "localized port a";
"Add.PortIn.b" = "localized port b";
"Add.PortOut.out" = "localized port out";
"Add.OIP.Multiplier" = "localized OIP name";
"Add.OIP.Popup" = "localized popup OIP name";
"Add.OIPChoice.choice 1" = "localized choice 1";
"Add.OIPChoice.choice 2" = "localized choice 2";
```

# Tips

There is a list of useful tips that will help you design and implement a node.

## Types

Always design your code to take care of any value types on the input ports. It is never guaranteed what kind of values will be passed in as it is unknown how this node will be used in a network.

# See Also

[Marionette Basics](Basics.md) | [Python](../../Python/README.md) | [Python#How to start with Python](../../Python/README.md#how-to-start-with-python) | [Function Reference](../../Function%20Reference/README.md)
