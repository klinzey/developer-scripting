# GetObjTypeProperties

## Description
Receives an object type and returns the properties of that object type

```pascal
FUNCTION GetObjTypeProperties(ObjectType : INTEGER) : INTEGER;
```

```python

def vs.GetObjTypeProperties(ObjectType):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|ObjectType|INTEGER|Object type whose properties are desired|

## Returns
Returns bit map of properties associated with an object's type

## Examples
```pascal
This function should return kTermProp for type kTermNode, kLineProp for kLineNode and so on for all existing object types that are defined in Objs.TDType.h.
```

## Version
Availability: from Vectorworks 2018
## Category
* Object Attributes

