# DBObjSQLSetWrite

## Description
Set an object's SQL sentence for ODBC write.

```pascal
FUNCTION DBObjSQLSetWrite(
				hObject     : HANDLE;
				SQLSentence : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBObjSQLSetWrite(hObject, SQLSentence):
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

