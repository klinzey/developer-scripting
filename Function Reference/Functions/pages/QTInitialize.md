# QTInitialize

## Description
Initializes QuickTime and returns the QuckTime version number.

```pascal
FUNCTION QTInitialize : INTEGER;
```

```python

def vs.QTInitialize():
    return INTEGER
```

## Returns
Returns the QuickTime version number. A value of 0 indicates QuickTime is not available.

## Remarks
We don't support QuickTime versions less than 3.0, so this function will return 0 in that scenario.

## Version
Availability: from VectorWorks8.5
## Category
* Special - QuickTime

