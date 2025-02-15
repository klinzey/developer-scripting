# GetWSCellTextFormat

## Description
Returns text format settings for a cell in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Text Style&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Style&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plain&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bold&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Italic&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Underline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Outline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;8&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Shadowed&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;16&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Superscript&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;32&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Subscript&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;64&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE GetWSCellTextFormat(
				worksheet     : HANDLE;
				row           : INTEGER;
				column        : INTEGER;
				VAR fontIndex : INTEGER;
				VAR size      : INTEGER;
				VAR style     : INTEGER);
```

```python

def vs.GetWSCellTextFormat(worksheet, row, column):
    return (fontIndex, size, style)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|row|INTEGER|Row of cell to be queried.|
|column|INTEGER|Column of cell to be queried.|
|fontIndex|INTEGER|Font index of cell text.|
|size|INTEGER|Font size of cell text.|
|style|INTEGER|Font style of cell text.|

## Remarks
Text Format (style) constants:<BR>
Plain              = 0<BR>
Bold              = 1<BR>
Italic             = 2<BR>
Underline    = 4<BR>
Outline         = 8<BR>
Shadow       = 16<BR>
<BR>
Note: Outline and Shadow only display on the Mac

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets

