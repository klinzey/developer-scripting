# DBObjSQLGetRead

## Description
Get an object's SQL sentence for ODBC read.

```pascal
FUNCTION DBObjSQLGetRead(
				hObject         : HANDLE;
				VAR SQLSentence : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBObjSQLGetRead(hObject):
    return (BOOLEAN, SQLSentence)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE||
|SQLSentence|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* ODBC

