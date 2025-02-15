# ForEachObjectInList

## Description
Processes all items in the specified list and and applies the specified action to each item.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - ForEachObjectInList Selectors&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133&gt;&lt;B&gt;&lt;I&gt;Object Options&lt;/I&gt;&lt;/B&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48&gt;&amp;nbsp;&lt;/TD&gt;
	&lt;TD WIDTH=297&gt;&amp;nbsp;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH WIDTH=133&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Option &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=48&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=297&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/THD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		All objects  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		0  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Visible Objects only  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		1  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Selected Objects only  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		2  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Locked objects only  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		4  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD WIDTH=48&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD WIDTH=297&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133&gt; &lt;DIV ALIGN=LEFT&gt; &lt;B&gt;&lt;I&gt;Traversal Options&lt;/I&gt;&lt;/B&gt;  
	  &lt;/DIV&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD WIDTH=297&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH WIDTH=133&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Option &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=48&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=297&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Traverse Shallow &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		0 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Traverse Groups  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		1  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Traverse inside groups  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Traverse Deep  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		2  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Traverse all containers (walls, extrudes, sweeps, etc)  
	  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE ForEachObjectInList(
				actionFunc  : PROCEDURE;
				objOptions  : INTEGER;
				travOptions : INTEGER;
				list        : HANDLE);
```

```python

def vs.ForEachObjectInList(actionFunc, objOptions, travOptions, list):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|actionFunc|PROCEDURE|Subroutine which performs operation on found objects.|
|objOptions|INTEGER|Object selection option index.|
|travOptions|INTEGER|Search options index.|
|list|HANDLE|Handle to first item in list.|

## Examples
```pascal
PROCEDURE Example;

CONST

   pioName = 'Complex Window 2';

   parameter = 'MeasureHeight';

   value = 'Head of Window';

   

FUNCTION DoIt(h :HANDLE) :BOOLEAN;

BEGIN

   h := FInSymDef(h);

   SetRField(h, pioName, parameter, value);

END;



BEGIN

    ForEachObjectInList(DoIt, 0, 0, FSymDef);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks8.5
## Category
* Utility

