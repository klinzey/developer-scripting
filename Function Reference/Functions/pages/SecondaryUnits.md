# SecondaryUnits

## Description
Procedure SecondaryUnits sets the secondary unit parameters for the active document. The secondary units setting is used primarily for display of alternate dimensions in&lt;BR&gt;
when a dual dimension standard is active. &lt;BR&gt;
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
PROCEDURE SecondaryUnits(
				style    : INTEGER;
				dimPrec  : LONGINT;
				format   : INTEGER;
				showMark : BOOLEAN;
				dispFrac : BOOLEAN);
```

```python

def vs.SecondaryUnits(style, dimPrec, format, showMark, dispFrac):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|style|INTEGER|Active secondary unit style for document.|
|dimPrec|LONGINT|Dimension precision.|
|format|INTEGER|Decimal formatting.|
|showMark|BOOLEAN|Unit mark display setting.|
|dispFrac|BOOLEAN|Fractional display setting.|

## Examples
```pascal
SecondaryUnits(1,6,2,TRUE,TRUE); 



{ Sets the secondary units to feet/inches with a dimension precision of 1/64, }

{ unit mark displayed, and fractional display of units values enabled.        }


```

## Version
Availability: from MiniCAD7.0
## Category
* Units

