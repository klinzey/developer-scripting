# GetSymbolOptionsN

## Description
Returns default class, insert  options, and break options for the specified symbol. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Symbol Insertion Options&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TD ROWSPAN=3 ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Insertion Mode&lt;/TD&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Description&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant 
	  Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Insert on Center Line&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Insert on Edge&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ROWSPAN=6 ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Break Mode&lt;/TD&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Description&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH  ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant 
	  Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Full Break with Caps&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Full Break No Caps&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Half Break&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;No Break&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE GetSymbolOptionsN(
				name           : STRING;
				VAR insertMode : INTEGER;
				VAR breakMode  : INTEGER;
				VAR className  : STRING);
```

```python

def vs.GetSymbolOptionsN(name):
    return (insertMode, breakMode, className)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|Name of symbol.|
|insertMode|INTEGER|Returns insertion mode of symbol.|
|breakMode|INTEGER|Returns break mode of symbol.|
|className|STRING|Default class of symbol.|

## Remarks
Gets the insertion options from the master symbol named &lt;name&gt;.<BR>
<BR>
See SetSymbolOptions.<BR>
<BR>
[8/18/98]

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Symbols

