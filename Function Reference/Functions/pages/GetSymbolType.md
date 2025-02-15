# GetSymbolType

## Description
Determines the type of the specified symbol instance.  The return values are:&lt;BR&gt;
0 - 2D Only&lt;BR&gt;
1 - 3D Only&lt;BR&gt;
2 - Hybrid

```pascal
FUNCTION GetSymbolType(objectHandle : HANDLE) : INTEGER;
```

```python

def vs.GetSymbolType(objectHandle):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to a symbol instance. |

## Returns
-1 = error.  Possibly wrong type of object passed in.<BR>
0 = 2D Symbol<BR>
1 = 3D Symbol<BR>
2 = Hybrid Symbol

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Symbols

