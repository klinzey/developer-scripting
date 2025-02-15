# SetLinkHeightToLayerDeltaZ

## Description
Sets whether or not the wall's height is linked to the layer delta z.

```pascal
FUNCTION SetLinkHeightToLayerDeltaZ(
				theWall           : HANDLE;
				linkToLayerDeltaZ : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetLinkHeightToLayerDeltaZ(theWall, linkToLayerDeltaZ):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall.|
|linkToLayerDeltaZ|BOOLEAN|Whether or not the wall's height is linked to the layer delta z.|

## Returns
Returns success status.

## See Also
VS Functions:
[GetLinkHeightToLayerDeltaZ](GetLinkHeightToLayerDeltaZ.md)

## Version
```diff
- SetLinkHeightToLayerDeltaZ is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.5
## Category
* Objects - Walls

