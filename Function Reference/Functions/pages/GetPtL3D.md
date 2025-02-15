# GetPtL3D

## Description
Procedure GetPtL3D creates a temporary &amp;quot;rubberband&amp;quot; 3D line from a specified point to the user selected end point. This cannot be used if there is a function anywhere in the calling chain. 

```pascal
PROCEDURE GetPtL3D(
				p1        : REAL;
				VAR p2    : REAL;
				useWPOnly : BOOLEAN);
```

```python

def vs.GetPtL3D(p1, useWPOnly):
    return p2
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Coordinates of line start point.|
|p2|REAL|Returns coordinates of mouse click.|
|useWPOnly|BOOLEAN|TRUE if the returned point have to be on the active Working Plane. Snapping to arbitrary 3D geometry will produce vertical projection result on the WP; FALSE if the point can be arbitrary 3D point (produced, for example, by snapping to a 3D geometry)|

## See Also
VS Functions:
[GetPt](GetPt.md)| [GetPtL](GetPtL.md)| [GetLine](GetLine.md)| [GetRect](GetRect.md)| [GetPt3D](GetPt3D.md)| [GetPtL3D](GetPtL3D.md)| [GetLine3D](GetLine3D.md)| [GetRect3D](GetRect3D.md)

## Version
Availability: from Vectorworks 2010
## Category
* User Interactive

