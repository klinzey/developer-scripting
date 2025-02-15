# SetComponentUsePenClassAttr

## Description
Sets the use class attributes flags of the pens of a component in an object.

```pascal
FUNCTION SetComponentUsePenClassAttr(
				object                     : HANDLE;
				componentIndex             : INTEGER;
				useLeftPenClassAttributes  : BOOLEAN;
				useRightPenClassAttributes : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetComponentUsePenClassAttr(object, componentIndex, useLeftPenClassAttributes, useRightPenClassAttributes):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|useLeftPenClassAttributes|BOOLEAN|Whether or not the component will use class attributes for its left pen.|
|useRightPenClassAttributes|BOOLEAN|Whether or not the component will use class attributes for its right pen.|

## See Also
VS Functions:
[GetComponentUsePenClassAttr](GetComponentUsePenClassAttr.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural

