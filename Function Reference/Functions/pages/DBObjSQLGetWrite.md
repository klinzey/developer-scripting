# DBObjSQLGetWrite

## Description
Get an object's SQL sentence for ODBC write.

```pascal
FUNCTION DBObjSQLGetWrite(
				hObject         : HANDLE;
				VAR SQLSentence : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBObjSQLGetWrite(hObject):
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

