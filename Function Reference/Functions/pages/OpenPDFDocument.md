# OpenPDFDocument

## Description
Begins the export to a PDF document.  You must call AcquireExportPDFSettingsAndLocation before calling this function. This is intended to support Batch PDF Export.

```pascal
FUNCTION OpenPDFDocument(inFilenameStr : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.OpenPDFDocument(inFilenameStr):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inFilenameStr|DYNARRAY[] of CHAR||

## Version
Availability: from VectorWorks12.5
## Category
* Command

