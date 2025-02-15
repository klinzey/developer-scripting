# GetCompAltSecFill

## Description
Gets the alternate section fill of a component in an object.

```pascal
FUNCTION GetCompAltSecFill(
				object                   : HANDLE;
				componentIndex           : INTEGER;
				VAR alternateSectionFill : LONGINT) : BOOLEAN;
```

```python

def vs.GetCompAltSecFill(object, componentIndex):
    return (BOOLEAN, alternateSectionFill)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a roof face, roof, Roof Style, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|alternateSectionFill|LONGINT|Returns the alternate section fill of the component.|

## See Also
VS Functions:
[SetCompAltSecFill](SetCompAltSecFill.md)

## Version
Availability: from Vectorworks 2016
## Category
* Objects - Architectural

