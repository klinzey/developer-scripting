# CalcVolume

## Description
Function CalcVolume calculates the volume of the referenced solid object. The function supports only valid solids objects.

```pascal
FUNCTION CalcVolume(solidObject : HANDLE) : REAL;
```

```python

def vs.CalcVolume(solidObject):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|solidObject|HANDLE|Handle to solids object.|

## Remarks
Calculates the volume of the given object if a valid solid.

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
```diff
- CalcVolume is obsolete as of VectorWorks12.5
```

Availability: from VectorWorks8.0
## Category
* Objects - Solids

