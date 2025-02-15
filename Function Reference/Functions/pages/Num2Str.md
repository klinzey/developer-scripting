# Num2Str

## Description
Function Num2Str converts a REAL value to a string and returns the value.&lt;BR&gt;
&lt;BR&gt;
Parameter decPlace has a range of -1 to 10; if -1 is specified, the value will be returned in scientific notation.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Num2Str(
				decPlace : INTEGER;
				v        : REAL) : STRING;
```

```python

def vs.Num2Str(decPlace, v):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|decPlace|INTEGER|Number of decimal places.|
|v|REAL|Numeric value.|

## Examples
```pascal
oldnumValue:=232.5148;

newStrValue:=Num2Str(3,oldnumValue);

{would return '232.515'}
```

## Version
Availability: from MiniCAD
## Category
* Strings

