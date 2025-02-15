# CreateTile

## Description
Creates a new tile resource.

```pascal
FUNCTION CreateTile(tileName : DYNARRAY[] of CHAR) : HANDLE;
```

```python

def vs.CreateTile(tileName):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|tileName|DYNARRAY[] of CHAR|A user-specified name by which the newly created tile will be identified.|

## Returns
Returns a handle to a new tile resource if successful, otherwise the function returns nil.

## Examples
```pascal
tileHandle := CreateTile('My Tile');
```

## See Also
VS Functions:
[CreateTile](CreateTile.md)| [ShowEditTileDialog](ShowEditTileDialog.md)| [ShowEditTileSettingsDialog](ShowEditTileSettingsDialog.md)| [ShowNewTileDialog](ShowNewTileDialog.md)| [GetTileGeometryGroup](GetTileGeometryGroup.md)| [BeginGroupN](BeginGroupN.md)| [AddTileGeometryObject](AddTileGeometryObject.md)| [GetTileGroupParent](GetTileGroupParent.md)| [IsTileGroupContainedObject](IsTileGroupContainedObject.md)| [GetTileBackgroundColor](GetTileBackgroundColor.md)| [SetTileBackgroundColor](SetTileBackgroundColor.md)| [GetTileRepetitionPoint](GetTileRepetitionPoint.md)| [SetTileRepetitionPoint](SetTileRepetitionPoint.md)| [GetTileOffsetPoint](GetTileOffsetPoint.md)| [SetTileOffsetPoint](SetTileOffsetPoint.md)

## Version
Availability: from Vectorworks 2011
## Category
* Document Attributes

