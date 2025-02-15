# SetBinaryConstraint

## Description
Applies a binary parametric constraint to the referenced objects. The geometry of the constraint is defined by the specified object vertices. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Binary Constraint Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt;&lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt;&lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Constraint Type&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		1 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;coincident&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		2 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;collinear&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		3 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;parallel &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		6 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;tangent &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		7 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;concentric&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		8 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;distance &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		9 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;horizontal distance&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		10 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;vertical distance&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		12 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;angle&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		13 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;perpendicular&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
To apply a constraint to an object within a symbol, use GetClosestPt to obtain an index to the object and pass the index to either obj2VertA to use it as the first object or obj2VertB to use it as the second object. In all other instances, pass 0 to both these parameters.

```pascal
FUNCTION SetBinaryConstraint(
				typeOfConstraint : INTEGER;
				h1               : HANDLE;
				h2               : HANDLE;
				obj1VertA        : INTEGER;
				obj1VertB        : INTEGER;
				obj2VertA        : INTEGER;
				obj2VertB        : INTEGER;
				containedObj1    : LONGINT;
				containedObj2    : LONGINT) : BOOLEAN;
```

```python

def vs.SetBinaryConstraint(typeOfConstraint, h1, h2, obj1VertA, obj1VertB, obj2VertA, obj2VertB, containedObj1, containedObj2):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|typeOfConstraint|INTEGER|Type of constraint to be applied.|
|h1|HANDLE|Handle to object accepting constraint.|
|h2|HANDLE|Handle to object accepting constraint.|
|obj1VertA|INTEGER|Vertex on first object defining constraint geometry.|
|obj1VertB|INTEGER|Vertex on first object defining constraint geometry.|
|obj2VertA|INTEGER|Vertex on second object defining constraint geometry.|
|obj2VertB|INTEGER|Vertex on second object defining constraint geometry.|
|containedObj1|LONGINT|Object index, obtained from the GetClosestPt function.|
|containedObj2|LONGINT|Object index, obtained from the GetClosestPt function.|

## Returns
Returns a BOOLEAN value indicating whether the constraint was successfully applied.

## Remarks
Sets a constraint on h1 and h2 on the designated vertices.  Valid values for typeOfConstraint are 1 (coincident), 2 (colinear), 3 (parallel), 6 (tangent), 7 (concentric), 8 (distance), 9 (horizontal distance), 10 (vertical distance), 12 (angle) and 13 (perpendicular).  obj1VertA and obj1VertB indicate which vertices of the first object to use in the constraint, and obj2VertA and obj2VertB indicate which vertices of the second object to use.  A value of -1 indicates that a vertex parameter is not applicable. The containedObj fields are for an index into the list of a container object such as a symbol.  This can be obtained from the GetClosestPt function.

## Version
Availability: from VectorWorks9.0
## Category
* Parametric Constraints

