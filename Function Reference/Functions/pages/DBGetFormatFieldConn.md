# DBGetFormatFieldConn

## Description
Get ODBC connection for the specified format field.

```pascal
FUNCTION DBGetFormatFieldConn(
				formatName     : STRING;
				VAR fieldName  : STRING;
				VAR columnName : STRING;
				VAR linkType   : INTEGER) : BOOLEAN;
```

```python

def vs.DBGetFormatFieldConn(formatName):
    return (BOOLEAN, fieldName, columnName, linkType)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|formatName|STRING||
|fieldName|STRING||
|columnName|STRING||
|linkType|INTEGER||

## Version
Availability: from Vectorworks 2011
## Category
* ODBC

