# MoveObjs

## Description
Procedure MoveObjs moves object(s) a specified offset distance. The last two parameters, allLayers and allObjects,  control which objects are offset by this procedure.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Effect of MoveObjs Parameters&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;allLayers&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;allObjects&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Effect&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;TRUE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;TRUE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;Move all objects on all layers&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;TRUE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;FALSE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;Move selected objects on all layers&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;FALSE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;TRUE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;Move all objects on active layer&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;FALSE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;FALSE&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;Move selected objects on active layer&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;


```pascal
PROCEDURE MoveObjs(
				move       : REAL;
				allLayers  : BOOLEAN;
				allObjects : BOOLEAN);
```

```python

def vs.MoveObjs(move, allLayers, allObjects):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|move|REAL|X-Y object offset distance.|
|allLayers|BOOLEAN|Move objects on all layers option setting.|
|allObjects|BOOLEAN|Move all objects option setting.|

## Examples
```pascal
MoveObjs(3,0,FALSE,FALSE);

{ moves selected objects on active layer 3 units to the right }


```

## Version
Availability: from MiniCAD
## Category
* Object Editing

