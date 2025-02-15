# GetFolder

## Description
Gets the path to a user selected folder

```pascal
FUNCTION GetFolder(
				promptStr         : STRING;
				VAR directoryPath : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.GetFolder(promptStr):
    return (INTEGER, directoryPath)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|promptStr|STRING||
|directoryPath|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2014
## Category
* File I/O

