# GetCWFramesFromPt

## Description
Returns information about the frames in a curtain wall from a given point.&lt;BR&gt;
&lt;BR&gt;
Used for placing objects inside a panel in a curtain wall. When passing the center point of the object in the wall, it will find the panel in the curtain wall and return information about the surrounding frames.

```pascal
FUNCTION GetCWFramesFromPt(
				hWall                : HANDLE;
				testPt               : REAL;
				includeBottomFrame   : BOOLEAN;
				VAR panelThickness   : REAL;
				VAR panelOffset      : REAL;
				VAR frameInsetTop    : REAL;
				VAR frameInsetBottom : REAL;
				VAR frameInsetRight  : REAL;
				VAR frameInsetLeft   : REAL) : BOOLEAN;
```

```python

def vs.GetCWFramesFromPt(hWall, testPt, includeBottomFrame):
    return (BOOLEAN, panelThickness, panelOffset, frameInsetTop, frameInsetBottom, frameInsetRight, frameInsetLeft)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hWall|HANDLE|Handle to the curtain wall|
|testPt|REAL|Point to test on the curtain wall. Typically the center point of the object to be placed in the curtain wall panel.|
|includeBottomFrame|BOOLEAN|Include the bottom frame.|
|panelThickness|REAL|This is the thickness of the panel as it subtracts from the frames. It is a property of the panel|
|panelOffset|REAL|This is the dimension from the center of the panel to the center of the wall|
|frameInsetTop|REAL|The frame inset is the distance the panel extends into and subtracts from the frame. |
|frameInsetBottom|REAL||
|frameInsetRight|REAL||
|frameInsetLeft|REAL||

## Returns
Returns TRUE if hWall is a curtain wall and frames are found.<BR>
Returns FALSE is hWall is not a curtain wall or the test point is not found on the wall.

## Version
Availability: from Vectorworks 2015
## Category
* Objects - Walls

