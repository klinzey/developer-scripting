# SetTopPlan2DComp

## Description
Sets the 2D component that is shown in Top/Plan view for a symbol definition or plug-in object&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Components&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Component&lt;/FONT&gt;&lt;/TH&gt;
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top and Bottom Cut&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION SetTopPlan2DComp(
				objectHandle : HANDLE;
				component    : INTEGER) : BOOLEAN;
```

```python

def vs.SetTopPlan2DComp(objectHandle, component):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to the object.|
|component|INTEGER|2D component to be shown in Top/Plan view.|

## Returns
Returns TRUE if the operation was successful. 

## See Also
VS Functions:
[GetTopPlan2DComp](GetTopPlan2DComp.md)| [Set2DComponentGroup](Set2DComponentGroup.md)| [Get2DComponentGroup](Get2DComponentGroup.md)

## Version
Availability: from Vectorworks 2019
## Category
* Objects - Custom

