# EA_DataAccCompGet

## Description
Gets object component data.

```pascal
PROCEDURE EA_DataAccCompGet(
				acc              : INTEGER;
				componentIndex   : INTEGER;
				VAR outInclude   : BOOLEAN;
				VAR outLambda    : REAL;
				VAR outThickness : REAL);
```

```python

def vs.EA_DataAccCompGet(acc, componentIndex):
    return (outInclude, outLambda, outThickness)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|acc|INTEGER||
|componentIndex|INTEGER||
|outInclude|BOOLEAN||
|outLambda|REAL||
|outThickness|REAL||

## Version
Availability: from Vectorworks 2016
## Category
* EnergyAnalysis Interface Library

