# PrimaryUnits

## Description
Procedure PrimaryUnits specifies the primary units settings for the active document. The primary units setting is used by the document for all measurement entry and display values in the document. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Standard Unit Settings&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
	&lt;TABLE BORDER=&quot;0&quot; ALIGN=&quot;CENTER&quot; CELLSPACING=&quot;1&quot; CELLPADDING=&quot;3&quot; ID=&quot;Table1&quot;&gt;
		&lt;TR&gt;
			&lt;TH ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#000000&quot;&gt;
				&lt;FONT COLOR=&quot;#FFFFFF&quot;&gt;Units Setting&lt;/FONT&gt;&lt;/TH&gt;
			&lt;TH ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#000000&quot;&gt;
				&lt;FONT COLOR=&quot;#FFFFFF&quot;&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Custom&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;0&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Feet/Inches&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;1&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Inches&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;2&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Feet&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;3&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Yards&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;4&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Miles&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;5&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Microns&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;6&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Millimeters&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;7&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Centimeters&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;8&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Meters&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;9&lt;/TD&gt;
		&lt;/TR&gt;
		&lt;TR&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCCC&quot;&gt;Kilometers&lt;/TD&gt;
			&lt;TD ALIGN=&quot;CENTER&quot; BGCOLOR=&quot;#CCCCFF&quot;&gt;10&lt;/TD&gt;
		&lt;/TR&gt;
	&lt;/TABLE&gt;
&lt;/CENTER&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Units Formats&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Units Format&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Decimal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fractional&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Decimal Ft/Inches&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fractional Ft/Inches&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE PrimaryUnits(
				style    : INTEGER;
				prec     : LONGINT;
				dimPrec  : LONGINT;
				format   : INTEGER;
				angPrec  : INTEGER;
				showMark : BOOLEAN;
				dispFrac : BOOLEAN);
```

```python

def vs.PrimaryUnits(style, prec, dimPrec, format, angPrec, showMark, dispFrac):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|style|INTEGER|Active primary unit style for document.|
|prec|LONGINT|Display precision.|
|dimPrec|LONGINT|Dimension precision.|
|format|INTEGER|Decimal formatting.|
|angPrec|INTEGER|Angular precision.|
|showMark|BOOLEAN|Unit mark display setting.|
|dispFrac|BOOLEAN|Fractional display setting.|

## Remarks
[sd 8/18/98]

## Examples
```pascal
PROCEDURE Example;

VAR

	style :INTEGER;

	prec, dimPrec :LONGINT;

	format, angPrec :INTEGER;

	showMark, dispFrac :BOOLEAN;

	outStr :STRING;

BEGIN

	outStr := '';

	GetPrimaryUnitInfo(style, prec, dimPrec, format, angPrec, showMark, dispFrac);

	FOR style := 0 to 16 DO BEGIN

		PrimaryUnits(style, prec, dimPrec, format, angPrec, showMark, dispFrac);

		outStr := Concat(outStr, Chr(13), style, ': ', GetPrefReal(152));

	END;

	AlrtDialog(outStr);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD7.0
## Category
* Units

