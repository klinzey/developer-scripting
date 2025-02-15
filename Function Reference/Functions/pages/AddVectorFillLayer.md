# AddVectorFillLayer

## Description
Procedure AddVectorFillLayer is used to add layers to a vector fill definition. This procedure call should follow a call to BeginVectorFillN. &lt;BR&gt;
&lt;BR&gt;
The input parameters for a vector fill layer match the inputs from the right side of the Vectorworks hatch editor dialog.&lt;BR&gt;
&lt;BR&gt;
A color table listing with associated index values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#colors&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE AddVectorFillLayer(
				xStart     : REAL;
				yStart     : REAL;
				xRepeat    : REAL;
				yRepeat    : REAL;
				xOffset    : REAL;
				yOffset    : REAL;
				dashFactor : REAL;
				lineWeight : INTEGER;
				colorIndex : INTEGER);
```

```python

def vs.AddVectorFillLayer(xStart, yStart, xRepeat, yRepeat, xOffset, yOffset, dashFactor, lineWeight, colorIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|xStart|REAL|X coordinate of fill origin.|
|yStart|REAL|Y coordinate of fill origin.|
|xRepeat|REAL|X coordinate of fill repeat origin.|
|yRepeat|REAL|Y coordinate of fill repeat origin.|
|xOffset|REAL|X coordinate of fill offset origin.|
|yOffset|REAL|Y coordinate of fill offset origin.|
|dashFactor|REAL|Dash factor of layer(percentage of fill line that is solid).|
|lineWeight|INTEGER|Line weight of layer, in mils.|
|colorIndex|INTEGER|Pen color of layer.|

## Remarks
Follows a call to BeginVectorFill. The input for the layer match the input from the right side of the hatch editor dialog.

## Examples
```pascal
PROCEDURE CreateHatch;

VAR

	hatchName :STRING;

BEGIN

	hatchName := 'My New Hatch';

	BeginVectorFillN(hatchName, TRUE, FALSE, 0);

	AddVectorFillLayer(0, 0, 1, 1, 0.1767767, -0.1767767, 1, 1, 255);

	EndVectorFill;

END;

RUN(CreateHatch);




```

## Version
Availability: from MiniCAD7.0.1
## Category
* Hatches / Vector Fills

