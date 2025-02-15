# GetVPLayerVisibility

## Description
Gets the visibility for the specified layer in the specified viewport.

```pascal
FUNCTION GetVPLayerVisibility(
				viewportHandle     : HANDLE;
				layerHandle        : HANDLE;
				VAR visibilityType : INTEGER) : BOOLEAN;
```

```python

def vs.GetVPLayerVisibility(viewportHandle, layerHandle):
    return (BOOLEAN, visibilityType)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE||
|layerHandle|HANDLE||
|visibilityType|INTEGER||

## Version
Availability: from VectorWorks11.0
## Category
* Objects - Groups

