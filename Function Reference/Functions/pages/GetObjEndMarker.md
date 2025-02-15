# GetObjEndMarker

## Description
Gets all properties for an object's end marker. Return TRUE if operation was successful.

```pascal
FUNCTION GetObjEndMarker(
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

def vs.GetObjEndMarker(object):
    return (BOOLEAN, style, angle, size, width, thicknessBasis, thickness, visibility)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|Handle to object.|
|style|LONGINT|The marker style. (see comments for details)|
|angle|INTEGER|The marker angle in degrees. (0 to 90)|
|size|REAL|The marker size in page inches.|
|width|REAL|The marker width in page inches.|
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

	ok := GetObjEndMarker (h, style, angle, size, width, thickBasis, thickness, visibility);

	Message (style, ' /  ', angle, '  /  ', size, '  /  ', width, ' /  ', thickBasis, ' /  ', thickness, ' /  ', visibility);

END;



RUN(Example);


```

## See Also
VS Functions:
[GetObjBeginningMarker](GetObjBeginningMarker.md)

## Version
Availability: from VectorWorks 2008
## Category
* Object Attributes

