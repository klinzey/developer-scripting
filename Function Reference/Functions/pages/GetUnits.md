# GetUnits

## Description
Procedure GetUnits returns the current units settings of the document.&lt;BR&gt;
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
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
More extensive Units information is available using the GetPref routines with the selectors shown in the tables of the VectorScript Appendix.

```pascal
PROCEDURE GetUnits(
				VAR fraction   : LONGINT;
				VAR display    : LONGINT;
				VAR format     : INTEGER;
				VAR upi        : REAL;
				VAR lenUnitMk  : STRING;
				VAR areaUnitMk : STRING);
```

```python

def vs.GetUnits():
    return (fraction, display, format, upi, lenUnitMk, areaUnitMk)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fraction|LONGINT|Approximate WorldCoords per drawing unit.  Use GetPrefReal(150) instead.  |
|display|LONGINT|Returns display accuracy.|
|format|INTEGER|Returns units format setting.|
|upi|REAL|Returns units per inch value.|
|lenUnitMk|STRING|Returns length unit mark.|
|areaUnitMk|STRING|Returns area unit mark.|

## Examples
```pascal
PROCEDURE Example;

VAR 

	fraction   :LONGINT; 

	display    :LONGINT; 

	format     :INTEGER; 

	upi        :REAL; 

	lenUnitMk   :STRING;

	areaUnitMk :STRING;

BEGIN

	GetUnits(fraction, display, format, upi, lenUnitMk, areaUnitMk);

	Message(fraction, ' ', display, ' ', format, ' ', upi, ' ', lenUnitMk, ' ', areaUnitMk);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Units

