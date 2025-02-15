# GetFileN

## Description
Returns the fully-qualified pathname of the selected file.

```pascal
FUNCTION GetFileN(
				title         : DYNARRAY[] of CHAR;
				defaultFolder : DYNARRAY[] of CHAR;
				mask          : DYNARRAY[] of CHAR;
				VAR fileName  : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.GetFileN(title, defaultFolder, mask):
    return (BOOLEAN, fileName)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|title|DYNARRAY[] of CHAR||
|defaultFolder|DYNARRAY[] of CHAR||
|mask|DYNARRAY[] of CHAR||
|fileName|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2014
## Category
* File I/O

