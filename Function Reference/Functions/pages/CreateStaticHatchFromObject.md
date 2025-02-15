# CreateStaticHatchFromObject

## Description
Creates a static hatch using inHatchName inside the bounds of the inObj.  The pX , pY and rotationAngle arguments determine the hatch origin and rotation used to generate the result.

```pascal
FUNCTION CreateStaticHatchFromObject(
				inObj         : HANDLE;
				inHatchName   : STRING;
				p             : REAL;
				rotationAngle : REAL) : HANDLE;
```

```python

def vs.CreateStaticHatchFromObject(inObj, inHatchName, p, rotationAngle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inObj|HANDLE|An object used as the boundary for the output.|
|inHatchName|STRING|The name of the hatch definition|
|p|REAL|A point specifying the origin of the output|
|rotationAngle|REAL|An angle specifying an offset angle to use to create the output|

## Returns
A group of lines in a hatch pattern as specified.

## Examples
```pascal
PROCEDURE Example;

VAR

	h:HANDLE;

	x,y:REAL;

BEGIN

GetPt(x,y);

h := CreateStaticHatchFromObject(FSActLayer,'Default Hatch', x, y, 0);

DSelectAll;

SetSelect(h);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks10.5
## Category
* Hatches / Vector Fills

