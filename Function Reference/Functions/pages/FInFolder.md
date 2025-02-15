# FInFolder

## Description
Function FInFolder returns a handle to the first object in the referenced symbol folder. The object can be either a symbol definition or a nested symbol folder.&lt;BR&gt;
If the folder is empty, the function returns NIL.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION FInFolder(sfHd : HANDLE) : HANDLE;
```

```python

def vs.FInFolder(sfHd):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|sfHd|HANDLE|Handle to symbol definition or symbol folder.|

## Version
Availability: from MiniCAD
## Category
* Document List Handling

