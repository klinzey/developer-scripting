# GetPickObjectInfo

## Description
Function GetPickObjectInfo returns a handle to an object found at a user selected point. &lt;BR&gt;
&lt;BR&gt;
Parameter subH returns a handle to a sub-selectable object (e.g., a symbol in a wall) if such an object exists. Parameter message is currently unused, and always returns 0.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetPickObjectInfo(
				p           : REAL;
				VAR h       : HANDLE;
				VAR subH    : HANDLE;
				VAR message : INTEGER) : BOOLEAN;
```

```python

def vs.GetPickObjectInfo(p):
    return (BOOLEAN, h, subH, message)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Coordinate location to test for object.|
|h|HANDLE|Returns handle to object.|
|subH|HANDLE|Returns handle to sub selectable object.|
|message|INTEGER|Resereved for future use. Specify a dummy INTEGER variable.|

## Remarks
same as PickObject except it return the sub-selected object, if any, and a message.  See Rich D. for more details.

## Examples
```pascal
WHILE NOT GetPickObjectInfo(pX,pY,hObject,hSymbol,dummyVar) DO BEGIN

    GetPt(pX,pY);

END;


```

## See Also
VS Functions:
[PickObject](PickObject.md)| [ForEachObjectAtPoint](ForEachObjectAtPoint.md)

## Version
Availability: from VectorWorks8.0
## Category
* Utility

