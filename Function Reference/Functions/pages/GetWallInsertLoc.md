# GetWallInsertLoc

## Description
Gets the wall insert location of a symbol definition, plug-in object style, or plug-in object.

```pascal
FUNCTION GetWallInsertLoc(hObject : HANDLE) : INTEGER;
```

```python

def vs.GetWallInsertLoc(hObject):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE|The symbol definition, plug-in object style, or plug-in object.|

## Returns
The wall insert location of the symbol definition, plug-in object style, or plug-in object.<BR>
<BR>
-1 - Insert on the nearest edge of the wall<BR>
0 - Insert on the center of the wall<BR>
1 - Insert on the left edge of the wall<BR>
2 - Insert on the right edge of the wall<BR>
3 - Insert on the center of the wall core component<BR>
4 - Insert on the left edge of the wall core component<BR>
5 - Insert on the right edge of the wall core component<BR>
6 - Insert on the wall insert location<BR>
7 - Insert on the wall closure insert location

## See Also
VS Functions:
[SetWallInsertLoc](SetWallInsertLoc.md)

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom

