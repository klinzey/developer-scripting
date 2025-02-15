# Generate2DFrom3DComp

## Description
Generates the specified 2D component of a symbol definition or plug-in object from the 3D component.&lt;BR&gt;
The resulting graphics will be similar to converting the 3D component to lines from a view corresponding to the 2D component view. &lt;BR&gt;
3D objects visible in the specified detail level will be used to generate the 2D component.&lt;BR&gt;
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
&lt;BR&gt;
&lt;I&gt;Table - Available Render Modes&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Render Mode&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Wireframe&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Hidden Line&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dashed Hidden Line&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;7&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Detail Levels&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Detail Level&lt;/FONT&gt;&lt;/TH&gt;
    &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Low&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Medium&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;High&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;All&lt;/TD&gt;
    &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;7&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION Generate2DFrom3DComp(
				objectHandle  : HANDLE;
				component     : INTEGER;
				renderMode    : INTEGER;
				levelOfDetail : INTEGER) : BOOLEAN;
```

```python

def vs.Generate2DFrom3DComp(objectHandle, component, renderMode, levelOfDetail):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle of a symbol or plug-in object.|
|component|INTEGER|2D component.|
|renderMode|INTEGER|Render mode.|
|levelOfDetail|INTEGER|Detail level. 3D objects visible in this detail level will be used to generate 2D component.|

## Returns
TRUE if the operation succeeded.

## See Also
VS Functions:
[Get2DComponentGroup](Get2DComponentGroup.md)| [Set2DComponentGroup](Set2DComponentGroup.md)

## Version
Availability: from Vectorworks 2019
## Category
* Objects - Custom

