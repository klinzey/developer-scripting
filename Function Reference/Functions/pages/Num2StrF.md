# Num2StrF

## Description
Function Num2StrF converts a specified REAL value into a string. The numeric value will be converted and displayed in the current unit settings of the drawing.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Num2StrF(vDistance : REAL (Coordinate)) : STRING;
```

```python

def vs.Num2StrF(vDistance):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|vDistance|REAL (Coordinate)|Numeric value.|

## Examples
```pascal
oldnumValue:=23.45;

newStrValue:=Num2StrF(oldnumValue);

{would return 1'-11 1/2&quot;}
```

## Version
Availability: from MiniCAD
## Category
* Strings

