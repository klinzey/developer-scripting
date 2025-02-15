# GetClUseGraphic

## Description
Returns whether the graphic attributes of the specified class will be used at object creation.

```pascal
FUNCTION GetClUseGraphic(className : STRING) : BOOLEAN;
```

```python

def vs.GetClUseGraphic(className):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|

## Returns
True indicates that this class is set to use its graphic attributes when objects are created in this class. False indicates that the objects created in this class will get default attributes from the default global attribute settings.

## Remarks
Returns whether the class is set to use its graphic attributes at object creation.

## Version
Availability: from VectorWorks8.0
## Category
* Classes

