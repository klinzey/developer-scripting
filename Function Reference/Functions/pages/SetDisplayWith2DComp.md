# SetDisplayWith2DComp

## Description
Sets whether a 3D object in a symbol definition or plug-in object is shown when the specified 2D component is shown.&lt;BR&gt;
&lt;BR&gt;
 &lt;I&gt;Table - 2D Components&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;2D Component&lt;/FONT&gt;&lt;/TH&gt;
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Not Set&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bottom&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top and Bottom Cut&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Front&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Back&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Front and Back Cut&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Left&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;7&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Right&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;8&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Left and Right Cut&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;9&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;


```pascal
FUNCTION SetDisplayWith2DComp(
				objectHandle : HANDLE;
				component    : INTEGER;
				isVisible    : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetDisplayWith2DComp(objectHandle, component, isVisible):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|3D object handle.|
|component|INTEGER|2D component.|
|isVisible|BOOLEAN|Visibility of the object when the 2D component is shown.|

## Returns
TRUE if the operation succeeded.

## See Also
VS Functions:
[Set2DComponentGroup](Set2DComponentGroup.md)| [Get2DComponentGroup](Get2DComponentGroup.md)

## Version
Availability: from Vectorworks 2019
## Category
* Objects - Custom

