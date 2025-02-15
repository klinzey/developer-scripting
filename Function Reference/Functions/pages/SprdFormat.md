# SprdFormat

## Description
Procedure SprdFormat determines the number format for cells within the active worksheet.&lt;BR&gt;
&lt;BR&gt;
Values for ldr and trailr may not exceed 8 characters.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Worksheet Cell Formats&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Cell Format&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;General&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Decimal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Decimal/comma&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Scientific&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fractional&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dimension&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Angle&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SprdFormat(
				numForm : INTEGER;
				acc     : INTEGER;
				ldr     : STRING;
				trailr  : STRING);
```

```python

def vs.SprdFormat(numForm, acc, ldr, trailr):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|numForm|INTEGER|Numeric format of cell.|
|acc|INTEGER|Numeric accuracy setting.|
|ldr|STRING|String prefix for cell.|
|trailr|STRING|String suffix for cell.|

## Remarks
OBSOLETE for Version 9: see new SetWSCellNumberFormat. [VML 01/09/01]

## Examples
```pascal
SprdFormat(2,2,'$','');

LoadCell(1,1,'=500 * 3.25');


```

## Version
```diff
- SprdFormat is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets

