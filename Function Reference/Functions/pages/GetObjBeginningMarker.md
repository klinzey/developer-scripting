# GetObjBeginningMarker

## Description
Gets all properties for an object's beginning marker. Return TRUE if operation was successful.

```pascal
FUNCTION GetObjBeginningMarker(
				object             : HANDLE;
				VAR style          : LONGINT;
				VAR angle          : INTEGER;
				VAR size           : REAL;
				VAR width          : REAL;
				VAR thicknessBasis : INTEGER;
				VAR thickness      : REAL;
				VAR visibility     : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetObjBeginningMarker(object):
    return (BOOLEAN, style, angle, size, width, thicknessBasis, thickness, visibility)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|Handle to object.|
|style|LONGINT|The marker style. (see comments for details)|
|angle|INTEGER|The marker angle in degrees. (0 to 90)|
|size|REAL|The marker size in inches.|
|width|REAL|The marker width in inches.|
|thicknessBasis|INTEGER|The marker thickness basis. ( see comments for details)|
|thickness|REAL|The marker thickness.|
|visibility|BOOLEAN|The marker visibility.|

## Examples
```pascal
PROCEDURE Example;

VAR

	h: HANDLE;

	style: INTEGER;

	angle: INTEGER;

	size: REAL;

	width: REAL;

	thickBasis: INTEGER;

	thickness: REAL;

	visibility: BOOLEAN;



	ok : BOOLEAN;

	

BEGIN

	h := FSActLayer;

	ok := GetObjBeginningMarker (h, style, angle, size, width, thickBasis, thickness, visibility);

	Message (style, ' /  ', angle, '  /  ', size, '  /  ', width, ' /  ', thickBasis, ' /  ', thickness, ' /  ', visibility);

END;



RUN(Example);


```

## See Also
VS Functions:
[GetObjEndMarker](GetObjEndMarker.md)

## Version
Availability: from VectorWorks 2008
## Category
* Object Attributes

