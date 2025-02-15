# TargetSprdSheet

## Description
Procedure TargetSprdSheet selects the referenced worksheet as the active worksheet for the document. The worksheet is not opened onscreen.

```pascal
PROCEDURE TargetSprdSheet(h : HANDLE);
```

```python

def vs.TargetSprdSheet(h):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|

## Remarks
This selects a spreadsheet for use by the script.  It does not open the spreadsheet. [sd 8/18/98]<BR>
OBSOLETE for Version 9: see new SetTopVisibleWS. [VML 01/09/01]

## Version
```diff
- TargetSprdSheet is obsolete as of VectorWorks9.0
```

Availability: from VectorWorks8.0
## Category
* Worksheets

