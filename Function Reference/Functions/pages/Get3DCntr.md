# Get3DCntr

## Description
Procedure Get3DCntr returns the three-dimensional center point of the referenced 3D object.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Get3DCntr(
				h          : HANDLE;
				VAR p      : REAL;
				VAR zValue : REAL);
```

```python

def vs.Get3DCntr(h):
    return (p, zValue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|p|REAL|Returns coordinates of object center point.|
|zValue|REAL|Returns elevation of object center point.|

## Examples
```pascal
PROCEDURE IncreaseExtr;

	{This script increases extruded objects in the selection by a user requested value.}

	{by Paolo, on the VectorScript bulletin board}

VAR

	oggetto :HANDLE;

	increaseValue :REAL;



FUNCTION Increase(h :HANDLE) :BOOLEAN;

VAR

	height, width, depth :REAL;

	xRot, yRot, zRot :REAL;

	p0X, p0Y, p0Z :REAL;

	p1X, p1Y, p1Z :REAL;

	result, isMirroredXY :BOOLEAN;

BEGIN

	{check if the obj is an extrusion}

	if (GetType(h) = 24) THEN BEGIN

		result := Get3DOrientation(h, xRot, yRot, zRot, isMirroredXY);

		Get3DCntr(h, p0X, p0Y, p0Z);

		

		SetRot3D(h, 0, 0, 0, 0, 0, 0);

		{here depth = extrusion value}

		Get3DInfo(h, height, width, depth);

		

		{I increase the depth}

		SET3DInfo(h, height, width, depth + increaseValue);



		SET3DRot(h, xRot, yRot, zRot , 0,0,0);

		

		Get3DCntr(h, p1X, p1Y, p1Z);

		

		{move of the misplacement p0-p1}

		Move3DObj(h, p0X-p1X, p0Y-p1Y, p0Z-p1Z);

		Get3DCntr(h, p1X, p1Y, p1Z);

	END;

	increase := FALSE;

END;



BEGIN

	{ask the value to increase}

	increaseValue := RealDialog('Increase extrusions in the selection of this value','10');

	{apply to the selected set of objects}

	ForEachObjectInList(increase, 2, 0, oggetto);

END;

RUN(IncreaseExtr);


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D

