# GetWSCellNumberFormat

## Description
Returns the numeric formatting of a cell in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
Specific index values for numeric formats and accuracy are listed in the Appendix.

```pascal
PROCEDURE GetWSCellNumberFormat(
				worksheet         : HANDLE;
				row               : INTEGER;
				column            : INTEGER;
				VAR style         : INTEGER;
				VAR accuracy      : INTEGER;
				VAR leaderString  : STRING;
				VAR trailerString : STRING);
```

```python

def vs.GetWSCellNumberFormat(worksheet, row, column):
    return (style, accuracy, leaderString, trailerString)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|row|INTEGER|Row of cell to be queried.|
|column|INTEGER|Column of cell to be queried.|
|style|INTEGER|Numeric format style index.|
|accuracy|INTEGER|Numeric accuracy / secondary format index.|
|leaderString|STRING|Leader string (where applicable).|
|trailerString|STRING|Trailer string (where applicable).|

## Remarks
Number Format constants:<BR>
style                       value                meaning of accuracy<BR>
General                   = 0<BR>
FixDecimal            = 1                       number of decimal places<BR>
DecwCommas       = 2                      number of decimal places<BR>
Scientific               = 3                       number of decimal places<BR>
Fractional              = 4                       largest displayed denominator<BR>
Dimension            = 5                       <BR>
Angle                      = 6                       corresponds to angular accuracy in units dialog<BR>
Date                         = 7                       <BR>
Conditonal           = 8

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets

