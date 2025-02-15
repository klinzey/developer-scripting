# DBDocGetDB

## Description
Returns a string representing a ';' delimited list of the databases currectly connected to the document.

```pascal
FUNCTION DBDocGetDB(VAR outDatabases : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.DBDocGetDB():
    return (BOOLEAN, outDatabases)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|outDatabases|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* ODBC

