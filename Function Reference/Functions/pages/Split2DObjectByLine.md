# Split2DObjectByLine

## Description
Splits objectHd along a line defined by the two points.

```pascal
PROCEDURE Split2DObjectByLine(
				objectHd    : HANDLE;
				p1          : REAL;
				p2          : REAL;
				VAR listHds : HANDLE);
```

```python

def vs.Split2DObjectByLine(objectHd, p1, p2):
    return listHds
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE||
|p1|REAL||
|p2|REAL||
|listHds|HANDLE||

## Examples
```pascal
PROCEDURE Example;

VAR

   polyHandle :HANDLE;

   lineHandle :HANDLE;

   resultHandle :HANDLE;

   begPt :VECTOR;

   endPt :VECTOR;

BEGIN

   CallTool(-204); polyHandle := FSActLayer;

   CallTool(-201); lineHandle := FSActLayer;

   GetSegPt1(lineHandle, begPt.x, begPt.y);

   GetSegPt2(lineHandle, endPt.x, endPt.y);

   Split2DObjectByLine(polyHandle, begPt.x, begPt.y, endPt.x, endPt.y, resultHandle);

   resultHandle := CreateDuplicateObject(resultHandle, NIL);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks12.0
## Category
* Graphic Calculation

