# GetPt3D

## Description
Procedure GetPt3D switches the cursor to 3D selection mode and allows the user to select a point in a VectorWorks document. This cannot be used if there is a function anywhere in the calling chain.

```pascal
PROCEDURE GetPt3D(
				VAR p     : REAL;
				useWPOnly : BOOLEAN);
```

```python

def vs.GetPt3D(useWPOnly):
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Returns coordinates of mouse click.|
|useWPOnly|BOOLEAN|TRUE if the returned point have to be on the active Working Plane. Snapping to arbitrary 3D geometry will produce vertical projection result on the WP; FALSE if the point can be arbitrary 3D point (produced, for example, by snapping to a 3D geometry)|

## See Also
VS Functions:
[GetPt](GetPt.md)| [GetPtL](GetPtL.md)| [GetLine](GetLine.md)| [GetRect](GetRect.md)| [GetPt3D](GetPt3D.md)| [GetPtL3D](GetPtL3D.md)| [GetLine3D](GetLine3D.md)| [GetRect3D](GetRect3D.md)

## Version
Availability: from Vectorworks 2010
## Category
* User Interactive

