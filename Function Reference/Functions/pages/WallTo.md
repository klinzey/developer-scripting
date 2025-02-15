# WallTo

## Description
Procedure WallTo creates a wall object in a Vectorworks document. WallTo begins the wall at the current graphics pen position, with the end point at the specified location.&lt;BR&gt;
&lt;BR&gt;
To explicitly set the start point of the wall, WallTo must be preceded by either Procedure MoveTo, LineTo, Wall, or WallTo. The procedure automatically performs a join/cleanup operation an intersection if the previous procedure was a wall creation procedure.

```pascal
PROCEDURE WallTo(p : REAL);
```

```python

def vs.WallTo(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|End point of wall.|

## Examples
```pascal
PROCEDURE Example;

VAR

	x1, y1, x2, y2 :REAL;

	resourceID :LONGINT;

	wallStyleCnt :INTEGER;

	wallStyleName :STRING;

	wallStyleHand :HANDLE;

BEGIN

	resourceID := BuildResourceList(127, 113, '', wallStyleCnt);

	IF wallStyleCnt &gt; 0 THEN BEGIN

		wallStyleName := GetNameFromResourceList(resourceID, 1);

		AlrtDialog(wallStyleName);

		wallStyleHand := ImportResourceToCurrentFile(resourceID, 1);

		SetWallPrefStyle(wallStyleName);

	END ELSE BEGIN

		SetWallWidth(3.5&quot;);

	END;

	GetPt(x1, y1);

	GetPtL(x1, y1, x2, y2);

	MoveTo(x1, y1);

	WallTo(x2, y2);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Walls

