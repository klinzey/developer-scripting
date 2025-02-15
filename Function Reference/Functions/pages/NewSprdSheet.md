# NewSprdSheet

## Description
Procedure NewSprdSheet creates a new worksheet in a Vectorworks document.&lt;BR&gt;


```pascal
PROCEDURE NewSprdSheet(
				name            : STRING;
				location        : REAL;
				rows            : INTEGER;
				columns         : INTEGER;
				showOnDrawing   : BOOLEAN;
				openAfterCreate : BOOLEAN);
```

```python

def vs.NewSprdSheet(name, location, rows, columns, showOnDrawing, openAfterCreate):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|Name of new worksheet.|
|location|REAL|Insertion point of worksheet.|
|rows|INTEGER|Number of rows.|
|columns|INTEGER|Number of columns.|
|showOnDrawing|BOOLEAN|Display worksheet in document.|
|openAfterCreate|BOOLEAN|Open worksheet after creation.|

## Remarks
OBSOLETE for Version 9: see new CreateWS and ShowWS. [VML 01/09/01]

## Examples
```pascal
NewSprdSheet('Window Schedule',12,24,5,8,TRUE,FALSE);
```

## Version
```diff
- NewSprdSheet is obsolete as of VectorWorks9.0
```

Availability: from VectorWorks8.0
## Category
* Worksheets

