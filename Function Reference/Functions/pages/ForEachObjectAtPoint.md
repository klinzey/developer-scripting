# ForEachObjectAtPoint

## Description
Performs an action for each object at the specified point in the drawing. This call was implemented to get past the practical limitations of PickObject, which only finds the topmost object. This call will find all of the objects at a given point.&lt;BR&gt;
&lt;BR&gt;
&amp;quot;actionFunc&amp;quot; should actually be a function, not a procedure as the declaration indicates.&lt;BR&gt;
&lt;BR&gt;
If the callback function returns FALSE, ForEachObjectAtPoint will not process any more objects at the specified point.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - ForEachObjectAtPoint Selectors&lt;/I&gt;&lt;P&gt;
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
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE ForEachObjectAtPoint(
				actionFunc  : PROCEDURE;
				objOptions  : INTEGER;
				travOptions : INTEGER;
				loc         : REAL;
				pickRadius  : REAL);
```

```python

def vs.ForEachObjectAtPoint(actionFunc, objOptions, travOptions, loc, pickRadius):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|actionFunc|PROCEDURE||
|objOptions|INTEGER||
|travOptions|INTEGER||
|loc|REAL||
|pickRadius|REAL||

## Examples
```pascal
PROCEDURE Example;

VAR

   gx1, gy1 : REAL;



FUNCTION DoIt(h1 :HANDLE) :BOOLEAN;

BEGIN

   DSelectAll;

   SetSelect(h1);

   Redraw;

   Wait(1);

END;



BEGIN

   GetPt(gx1, gy1);

   ForEachObjectAtPoint(DoIt, 0, 0, gx1, gy1, 5);

END;

RUN(Example);
```

## See Also
VS Functions:
[PickObject](PickObject.md)| [GetPickObjectInfo](GetPickObjectInfo.md)

## Version
Availability: from VectorWorks 2008
## Category
* Utility

