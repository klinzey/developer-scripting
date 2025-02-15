# SprdAlign

## Description
Procedure SprdAlign determines the alignment setting within a worksheet cell. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Worksheet Cell Alignment&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Alignment&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;General&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Left&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Right&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Center&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;
&lt;BR&gt;


```pascal
PROCEDURE SprdAlign(align : INTEGER);
```

```python

def vs.SprdAlign(align):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|align|INTEGER|Text alignment within worksheet cell.|

## Remarks
OBSOLETE for Version 9: see new SetWSCellAlignment. [VML 01/09/01]

## Examples
```pascal
SprdAlign(2);

LoadCell(3,3,'Cell 1,1');


```

## Version
```diff
- SprdAlign is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets

