# DBDocSetColKey

## Description
Get database table column to be as a key.

```pascal
FUNCTION DBDocSetColKey(
				databaseName : DYNARRAY[] of CHAR;
				tableName    : DYNARRAY[] of CHAR;
				columnName   : DYNARRAY[] of CHAR;
				setIsKey     : BOOLEAN) : BOOLEAN;
```

```python

def vs.DBDocSetColKey(databaseName, tableName, columnName, setIsKey):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|databaseName|DYNARRAY[] of CHAR||
|tableName|DYNARRAY[] of CHAR||
|columnName|DYNARRAY[] of CHAR||
|setIsKey|BOOLEAN||

## Version
Availability: from Vectorworks 2011
## Category
* ODBC

