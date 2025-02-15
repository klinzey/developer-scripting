# ForEachObjectInLayer

## Description
Traverses through all objects according to specified search options and applies the specified action to each object.  The 'actionFunc' procedure should return false to continue with next object, or return true to stop the traversal.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - ForEachObjectInLayer Selectors&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3 ID=&quot;Table1&quot;&gt;
	&lt;TR&gt; 
		&lt;TH&gt;&lt;DIV ALIGN=LEFT&gt;&lt;I&gt;Object Options&lt;/I&gt;&lt;/DIV&gt;&lt;/TH&gt;
		&lt;TH&gt;&amp;nbsp;&lt;/TH&gt;
		&lt;TH&gt;&amp;nbsp;&lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR BGCOLOR=#000000&gt; 
		&lt;TH&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Option &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;All objects  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;0  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp;&lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Visible Objects only  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;1  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Selected Objects only  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;2  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Unlocked objects only  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;4  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133&gt;&amp;nbsp; &lt;/TD&gt;
		&lt;TD WIDTH=48&gt;&amp;nbsp; &lt;/TD&gt;
		&lt;TD WIDTH=297&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TH WIDTH=133&gt; &lt;DIV ALIGN=LEFT&gt;&lt;I&gt;Traversal Options&lt;/I&gt;&lt;/DIV&gt;&lt;/TH&gt;
		&lt;TH WIDTH=48&gt;&amp;nbsp; &lt;/TH&gt;
		&lt;TH WIDTH=297&gt;&amp;nbsp; &lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR BGCOLOR=#000000&gt; 
		&lt;TH WIDTH=133&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Option &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH WIDTH=48&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH WIDTH=297&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Traverse Shallow &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;0 &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Traverse Groups  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;1  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Traverse inside groups  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Traverse Deep  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;2  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Traverse all containers (walls, extrudes, sweeps, etc)&lt;/CENTER&gt;&lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133&gt;&amp;nbsp; &lt;/TD&gt;
		&lt;TD WIDTH=48&gt;&amp;nbsp; &lt;/TD&gt;
		&lt;TD WIDTH=297&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TH WIDTH=133&gt; &lt;DIV ALIGN=LEFT&gt; &lt;I&gt;Layer Options&lt;/I&gt;&lt;/DIV&gt;&lt;/TH&gt;
		&lt;TH WIDTH=48&gt;&amp;nbsp; &lt;/TH&gt;
		&lt;TH WIDTH=297&gt;&amp;nbsp; &lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR BGCOLOR=#000000&gt; 
		&lt;TH WIDTH=133&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Option &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH WIDTH=48&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
		&lt;TH WIDTH=297&gt; &lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Current layer  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;0  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;All layers  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;1  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Visible layers  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;2  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Editable layers  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;4  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
	&lt;TR&gt; 
		&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;Snappable layers  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;8  &lt;/CENTER&gt;&lt;/TD&gt;
		&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE ForEachObjectInLayer(
				actionFunc   : PROCEDURE;
				objOptions   : INTEGER;
				travOptions  : INTEGER;
				layerOptions : INTEGER);
```

```python

def vs.ForEachObjectInLayer(actionFunc, objOptions, travOptions, layerOptions):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|actionFunc|PROCEDURE|Subroutine which performs operation on found objects.|
|objOptions|INTEGER|Object selection option index.|
|travOptions|INTEGER|Search options index.|
|layerOptions|INTEGER|Layer selection option index.|

## Examples
```pascal
PROCEDURE Example;



FUNCTION MakeItRed(h :HANDLE) :BOOLEAN;

VAR

	r, g, b :LONGINT;

BEGIN

	ColorIndexToRGB(7, r, g, b);

	SetFillBack(h, r, g, b);

END;

	

BEGIN

	ForEachObjectInLayer(MakeItRed, 2, 0, 4);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.5
## Category
* Utility

