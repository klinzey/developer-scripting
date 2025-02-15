# AddCustomTexPart

## Description
This procedure adds a custom texture part with the specified ID and name to the object.  Use partID starting at 100 to avoid conflicts with existing texture parts.

```pascal
PROCEDURE AddCustomTexPart(
				obj      : HANDLE;
				partID   : LONGINT;
				partName : STRING);
```

```python

def vs.AddCustomTexPart(obj, partID, partName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|The object to add a custom texture part to.|
|partID|LONGINT|The texture part ID.  Start at 100 to avoid conflicts with existing texture parts.|
|partName|STRING|The texture part name, which will be shown in the texturing UI.|

## Examples
```pascal
RemoveCustomTexParts(h);

AddCustomTexPart(h, 100, ‘Stringers’);

AddCustomTexPart(h, 200, ‘Treads’);


```

## Version
Availability: from Vectorworks 2017
## Category
* Textures

