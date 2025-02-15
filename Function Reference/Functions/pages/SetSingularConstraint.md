# SetSingularConstraint

## Description
Applies a parametric constraint to the referenced object. The geometry of the constraint is defined by the specified object vertices. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Constraint Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Index &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Constraint Type &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		4  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Vertical  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		5  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Horizontal  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		8  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Distance  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		9  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Vertical distance  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		10  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Horizontal distance  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		11  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Radius  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;


```pascal
FUNCTION SetSingularConstraint(
				typeOfConstraint : INTEGER;
				h                : HANDLE;
				vertexA          : INTEGER;
				vertexB          : INTEGER) : BOOLEAN;
```

```python

def vs.SetSingularConstraint(typeOfConstraint, h, vertexA, vertexB):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|typeOfConstraint|INTEGER|Type of constraint to be applied.|
|h|HANDLE|Handle to object accepting constraint.|
|vertexA|INTEGER|Vertex defining the constraint geometry.|
|vertexB|INTEGER|Vertex defining the constraint geometry.|

## Returns
Returns a BOOLEAN value indicating whether the constraint was applied successfully.

## Remarks
Sets a constraint of type typeOfConstraint on the object h.  The valid values for typeOfConstraint are  4 (vertical), 5 (horizontal), 8 (distance), 9 (vertical distance), 10 (horizontal distance) and 11 (radius).  vertexA and vertexB indicate which vertices of the object define the geometry to be constrained.  A value of -1 indicates that a vertex parameter is not applicable.  It returns false if the constraint cannot be set.

## Version
Availability: from VectorWorks9.0
## Category
* Parametric Constraints

