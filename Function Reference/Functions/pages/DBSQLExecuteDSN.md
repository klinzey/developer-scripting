# DBSQLExecuteDSN

## Description
Executes a SQL in the specified DSN registered in the ODBC manager. Note! The resultSetInstance have to be deleted with call to 'DBSQLExecuteDelete'

```pascal
FUNCTION DBSQLExecuteDSN(
				dsn                  : DYNARRAY[] of CHAR;
				userName             : DYNARRAY[] of CHAR;
				password             : DYNARRAY[] of CHAR;
				SQLQuery             : DYNARRAY[] of CHAR;
				VAR outColumnCnt     : LONGINT;
				VAR outResultSetInst : LONGINT) : BOOLEAN;
```

```python

def vs.DBSQLExecuteDSN(dsn, userName, password, SQLQuery):
    return (BOOLEAN, outColumnCnt, outResultSetInst)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dsn|DYNARRAY[] of CHAR||
|userName|DYNARRAY[] of CHAR||
|password|DYNARRAY[] of CHAR||
|SQLQuery|DYNARRAY[] of CHAR||
|outColumnCnt|LONGINT||
|outResultSetInst|LONGINT||

## Version
Availability: from Vectorworks 2011
## Category
* ODBC

