# GetDLComponentClass

## Description
Gets the class of the component at index in the Double Line Preferences.

```pascal
FUNCTION GetDLComponentClass(
				index              : INTEGER;
				VAR componentClass : LONGINT) : BOOLEAN;
```

```python

def vs.GetDLComponentClass(index):
    return (BOOLEAN, componentClass)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|componentClass|LONGINT|Returns the class of the component.|

## See Also
VS Functions:
[SetDLComponentClass](SetDLComponentClass.md)

## Version
Availability: from VectorWorks 2008
## Category
* Document Settings

