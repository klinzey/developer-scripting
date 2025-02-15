# SetSymbolOptionsN

## Description
Sets the default class, insert  options, and break options for the specified symbol. &lt;BR&gt;
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
PROCEDURE SetSymbolOptionsN(
				name       : STRING;
				insertMode : INTEGER;
				breakMode  : INTEGER;
				className  : STRING);
```

```python

def vs.SetSymbolOptionsN(name, insertMode, breakMode, className):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|Name of symbol.|
|insertMode|INTEGER|Insertion mode of symbol.|
|breakMode|INTEGER|Break mode for symbol.|
|className|STRING|Default class for symbol.|

## Remarks
Sets the insert and break options for the master symbol named &lt;name&gt;. <BR>
<BR>
The insertMode options are:<BR>
0 = insert on the center line of the wall<BR>
1 = insert on the edge of the wall<BR>
<BR>
The breakMode options are:<BR>
1 = Full break with caps, both edges of the wall are broken and cap lines close off the two broken portions of the wall.<BR>
2 = Full break with no caps, both edges of the wall  are broken and there are no cap lines.<BR>
3 = Half break, for edge insertions only, wall edge is broken on the same edge that the symbol is inserted on.<BR>
4 = No break, there is no break in the wall, the symbol is drawn on top of the wall.<BR>
<BR>
See also Get SymbolOptions<BR>
<BR>
[sd 8/18/98]<BR>
<BR>
The className should specify the name of a class that exists in the parent document. After a class is set, all instances of<BR>
this symbol will be marked as members of the class.

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Symbols

