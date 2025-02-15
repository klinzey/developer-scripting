# Set2DComponentGroup

## Description
Sets the specified 2D component group of a symbol definition or plug-in object.   Use Top/Plan if you want to add the group into the main container of the object.                                                                             &lt;BR&gt;
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
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top/Plan&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;10&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION Set2DComponentGroup(
				objectHandle : HANDLE;
				groupHandle  : HANDLE;
				component    : INTEGER) : BOOLEAN;
```

```python

def vs.Set2DComponentGroup(objectHandle, groupHandle, component):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to the object.|
|groupHandle|HANDLE|Handle to the graphics group. Can be a group or a single object. To delete the corresponding group provide NULL.|
|component|INTEGER|2D component.|

## Returns
Returns TRUE if the operation was successful. 

## See Also
VS Functions:
[Get2DComponentGroup](Get2DComponentGroup.md)

## Version
Availability: from Vectorworks 2019
## Category
* Objects - Custom

