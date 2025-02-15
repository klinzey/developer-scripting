# ValidAngStr

## Description
Function ValidAngStr returns TRUE if the specified value can be converted into a numeric angle value. If TRUE, the value (in decimal degrees) of the string is returned.&lt;BR&gt;


```pascal
FUNCTION ValidAngStr(
				str       : STRING;
				VAR value : REAL) : BOOLEAN;
```

```python

def vs.ValidAngStr(str):
    return (BOOLEAN, value)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|str|STRING|String value to be checked for angle validity.|
|value|REAL|Returns numeric angle value converted from input string.|

## Returns
Returns TRUE if the specified string can be converted into a angle value.

## Examples
```pascal
PROCEDURE Example;

VAR

	str :STRING;

	value :REAL;

BEGIN

	str := StrDialog('Enter the angle:', 'N10E');

	IF ValidAngStr(str, value) THEN Message(value);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Utility

