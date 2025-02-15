# GetCWPanelFromPt

## Description
Returns information about a panel in a curtain wall from a given point.&lt;BR&gt;
&lt;BR&gt;
Used for placing objects inside a panel in a curtain wall. When passing the center point of the object in the wall, it will find the panel in the curtain wall and return a new center point and the height and width of the panel.

```pascal
FUNCTION GetCWPanelFromPt(
				hWall              : HANDLE;
				testPt             : REAL;
				includeBottomFrame : BOOLEAN;
				VAR centerPt       : REAL;
				VAR width          : REAL;
				VAR height         : REAL) : BOOLEAN;
```

```python

def vs.GetCWPanelFromPt(hWall, testPt, includeBottomFrame):
    return (BOOLEAN, centerPt, width, height)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hWall|HANDLE|Handle to the curtain wall|
|testPt|REAL|Point to test on the curtain wall. Typically the center point of the object to be placed in the curtain wall panel.|
|includeBottomFrame|BOOLEAN|Include the bottom frame in the return height. |
|centerPt|REAL|Returns the center point of the rectangle in witch to place the object. |
|width|REAL|The width of the rectangle in which to place the object.|
|height|REAL|The height of the rectangle in which to place the object.|

## Returns
Returns TRUE if hWall is a curtain wall and a panel is found.<BR>
Returns FALSE is hWall is not a curtain wall or the test point is not found on the wall.

## Version
Availability: from Vectorworks 2014
## Category
* Objects - Walls

