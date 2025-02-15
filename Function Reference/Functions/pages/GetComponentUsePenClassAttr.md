# GetComponentUsePenClassAttr

## Description
Gets the use class attributes flags of the pens of a component in an object.

```pascal
FUNCTION GetComponentUsePenClassAttr(
				object                         : HANDLE;
				componentIndex                 : INTEGER;
				VAR useLeftPenClassAttributes  : BOOLEAN;
				VAR useRightPenClassAttributes : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetComponentUsePenClassAttr(object, componentIndex):
    return (BOOLEAN, useLeftPenClassAttributes, useRightPenClassAttributes)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|useLeftPenClassAttributes|BOOLEAN|Returns whether or not the component is using class attributes for its left pen.|
|useRightPenClassAttributes|BOOLEAN|Returns whether or not the component is using class attributes for its right pen.|

## See Also
VS Functions:
[SetComponentUsePenClassAttr](SetComponentUsePenClassAttr.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural

