# GetBinaryConstraint

## Description
Returns a handle to a binary parametric constraint applied to the referenced objects.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Binary Constraint Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt;&lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt;&lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Constraint Type&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		1 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;coincident&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		2 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;collinear&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		3 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;parallel &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		6 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;tangent &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		7 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;concentric&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		8 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;distance &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		9 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;horizontal distance&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		10 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;vertical distance&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		12 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;angle&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		13 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;perpendicular&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION GetBinaryConstraint(
				constrType    : INTEGER;
				obj1          : HANDLE;
				obj2          : HANDLE;
				obj1VertA     : INTEGER;
				obj1VertB     : INTEGER;
				obj2VertA     : INTEGER;
				obj2VertB     : INTEGER;
				containedObj1 : LONGINT;
				containedObj2 : LONGINT) : HANDLE;
```

```python

def vs.GetBinaryConstraint(constrType, obj1, obj2, obj1VertA, obj1VertB, obj2VertA, obj2VertB, containedObj1, containedObj2):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|constrType|INTEGER|Type of constraint to be returned.|
|obj1|HANDLE|Handle to first object in constraint relationship.|
|obj2|HANDLE|Handle to second object in constraint relationship.|
|obj1VertA|INTEGER|Vertex defining the constraint geometry of first object.|
|obj1VertB|INTEGER|Vertex defining the constraint geometry of first object.|
|obj2VertA|INTEGER|Vertex defining the constraint geometry of second object.|
|obj2VertB|INTEGER|Vertex defining the constraint geometry of second object.|
|containedObj1|LONGINT||
|containedObj2|LONGINT||

## Returns
Returns a HANDLE to the constraint if exists, otherwise returns NIL.

## Version
Availability: from VectorWorks9.0
## Category
* Parametric Constraints

