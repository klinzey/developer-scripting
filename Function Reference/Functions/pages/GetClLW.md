# GetClLW

## Description
Returns the line weight of the specified class.

```pascal
FUNCTION GetClLW(className : STRING) : INTEGER;
```

```python

def vs.GetClLW(className):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|

## Remarks
Returns the line weight of the class named className.

## Examples
```pascal
pbLineWt:= GetClLW('Property Bounds');
```

## Version
Availability: from VectorWorks8.0
## Category
* Classes

