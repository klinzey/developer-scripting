# GetLBHeaderTextWidth

## Description
Produces the width in pixels that will show the given string without truncation in a listbrowser column header.  This will provide a guaranteed appropriate width for InsertLBColumn.

```pascal
FUNCTION GetLBHeaderTextWidth(
				className        : STRING;
				allowForSortIcon : BOOLEAN) : INTEGER;
```

```python

def vs.GetLBHeaderTextWidth(className, allowForSortIcon):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING||
|allowForSortIcon|BOOLEAN||

## Version
Availability: from Vectorworks 2009
## Category
* Dialogs - Modern

