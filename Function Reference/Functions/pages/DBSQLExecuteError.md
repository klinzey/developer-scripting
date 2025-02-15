# DBSQLExecuteError

## Description
Return information about the last error occured in the ODBC API functions.

```pascal
FUNCTION DBSQLExecuteError(
				VAR message      : DYNARRAY[] of CHAR;
				VAR state        : DYNARRAY[] of CHAR;
				VAR code         : LONGINT;
				VAR internalDesc : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBSQLExecuteError():
    return (BOOLEAN, message, state, code, internalDesc)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|message|DYNARRAY[] of CHAR||
|state|DYNARRAY[] of CHAR||
|code|LONGINT||
|internalDesc|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2012
## Category
* ODBC

