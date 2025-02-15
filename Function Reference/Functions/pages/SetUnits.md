# SetUnits

## Description
Procedure SetUnits sets low-level unit values in a Vectorworks document. &lt;BR&gt;
&lt;BR&gt;
If only one of the units values is to be modified, GetUnits should be called first, and the values retrieved from that call should be passed back into SetUnits. &lt;BR&gt;
&lt;BR&gt;
To specify a standard units setting with default values, use Units. To specify a standard units setting, but with some modified values, use PrimaryUnit.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Vectorworks Unit Formats&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Units Format&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Format Flag&lt;/FONT&gt;&lt;/TH&gt;
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
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Decimal Feet and Inches&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Fractional Feet and Inches &lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE SetUnits(
				fraction   : LONGINT;
				display    : LONGINT;
				format     : INTEGER;
				upi        : REAL;
				name       : STRING;
				squareName : STRING);
```

```python

def vs.SetUnits(fraction, display, format, upi, name, squareName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fraction|LONGINT|Stored accuracy for the document.|
|display|LONGINT|Minimum display accuracy for the document.|
|format|INTEGER|Unit format style.|
|upi|REAL|Units per inch.|
|name|STRING|Unit label for displayed values|
|squareName|STRING|Squared unit label for displayed values.|

## Remarks
Sets low-level unit values. If only one of the values is desired to change, GetUnits should be called first, and the values retrieved from that call should be passed back into SetUnits. If a standard unit with default values is desired, the Units procedure should be used, not this one. If a standard unit with some modified values is desired, the PrimaryUnit procedure should be called, not this one.<BR>
<BR>
[sd 8/18/98]

## Examples
```pascal
SetUnits(4096,64,3,1.0,'&quot;','sq ft');
```

## Version
Availability: from MiniCAD
## Category
* Document Settings

