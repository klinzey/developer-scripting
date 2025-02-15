# DBObjSQLSetRead

## Description
Set an object's SQL sentence for ODBC read.

```pascal
FUNCTION DBObjSQLSetRead(
				hObject     : HANDLE;
				SQLSentence : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBObjSQLSetRead(hObject, SQLSentence):
    return BOOLEAN
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

