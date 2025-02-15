# ObjSurfaceArea

## Description
Function ObjSurfaceArea calculates the surface area of the referenced solid object. The function supports only valid solids objects.

```pascal
FUNCTION ObjSurfaceArea(solidObject : HANDLE) : REAL;
```

```python

def vs.ObjSurfaceArea(solidObject):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|solidObject|HANDLE|Handle to solids object.|

## Remarks
Calculates the surface area of the given object if a valid solid.

## Examples
```pascal
PROCEDURE Example;

VAR

        volume, area: REAL;

BEGIN

        IF FSActLayer &lt;&gt; NIL THEN BEGIN

                volume := CalcVolume(FSActLayer);

                area := CalcSurfaceArea(FSActLayer);

                Message('Volume ', volume, ', surface area ', area);

        END;

END;

RUN(Example);
```

## Version
Availability: from VectorWorks12.5
## Category
* Objects - Solids

