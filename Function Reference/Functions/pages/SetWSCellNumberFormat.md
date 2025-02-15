# SetWSCellNumberFormat

## Description
Sets the numeric formatting of a cell in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
SetWSCellNumberFormat allows numeric formatting to be set for a rectangular range of cells. To set the formatting of a single cell, specify identical values for the top/bottom and left/right range boundaries.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Worksheet Number Formats&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Style&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Meaning of Accuracy&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;General&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fixed Decimal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;number of decimal places&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;DecwCommas&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;number of decimal places&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Scientific&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;number of decimal places&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fractional&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;largest displayed denominator&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dimension&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Angle&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;corresponds to angular accuracy in units dialog&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Date&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;7&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Conditional&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;8&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dimension Area&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;11&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dimension Volume&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;12&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Text&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;13&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;


```pascal
PROCEDURE SetWSCellNumberFormat(
				worksheet     : HANDLE;
				topRow        : INTEGER;
				leftColumn    : INTEGER;
				bottomRow     : INTEGER;
				rightColumn   : INTEGER;
				style         : INTEGER;
				accuracy      : INTEGER;
				leaderString  : STRING;
				trailerString : STRING);
```

```python

def vs.SetWSCellNumberFormat(worksheet, topRow, leftColumn, bottomRow, rightColumn, style, accuracy, leaderString, trailerString):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|topRow|INTEGER|Top row of cell range.|
|leftColumn|INTEGER|Leftmost column of cell range.|
|bottomRow|INTEGER|Bottom row of cell range.|
|rightColumn|INTEGER|Rightmost column of cell range.|
|style|INTEGER|Numeric format style index.|
|accuracy|INTEGER|Numeric accuracy / secondary format index.|
|leaderString|STRING|Leader string (where applicable).|
|trailerString|STRING|Trailer string (where applicable).|

## Remarks
Number Format constants:<BR>
style                       value                meaning of accuracy<BR>
General                   = 0<BR>
FixDecimal            = 1                       number of decimal places<BR>
DecwCommas       = 2                      number of decimal places<BR>
Scientific               = 3                       number of decimal places<BR>
Fractional              = 4                       largest displayed denominator<BR>
Dimension            = 5                       <BR>
Angle                      = 6                       corresponds to angular accuracy in units dialog<BR>
Date                         = 7                       <BR>
Conditonal           = 8

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets

