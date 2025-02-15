# GetCVis

## Description
Returns the visibility status of the specified class.&lt;BR&gt;
&lt;BR&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Visibility&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Index Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Visible&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Hidden&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;-1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Grayed&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION GetCVis(className : STRING) : INTEGER;
```

```python

def vs.GetCVis(className):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|

## Returns
<CENTER>
<TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3>
  <TR> 
	<TH ALIGN=CENTER BGCOLOR=#000000><FONT COLOR=#FFFFFF>Visibility</FONT></TH>
	<TH ALIGN=CENTER BGCOLOR=#000000><FONT COLOR=#FFFFFF>Index Value</FONT></TH>
  </TR>
  <TR> 
	<TD ALIGN=CENTER BGCOLOR=#CCCCCC>Visible</TD>
	<TD ALIGN=CENTER BGCOLOR=#CCCCFF>0</TD>
  </TR>
  <TR> 
	<TD ALIGN=CENTER BGCOLOR=#CCCCCC>Hidden</TD>
	<TD ALIGN=CENTER BGCOLOR=#CCCCFF>-1</TD>
  </TR>
  <TR> 
	<TD ALIGN=CENTER BGCOLOR=#CCCCCC>Grayed</TD>
	<TD ALIGN=CENTER BGCOLOR=#CCCCFF>2</TD>
  </TR>
</TABLE>
</CENTER><BR>


## Examples
```pascal
PROCEDURE Example;

BEGIN

	Message(GetCVis('Dimension'));

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Classes

