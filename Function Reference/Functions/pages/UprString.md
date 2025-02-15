# UprString

## Description
Procedure UprString converts all characters in the specified string to upper case.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE UprString(VAR str : DYNARRAY[] of CHAR);
```

```python

def vs.UprString(str):
    return str
```

## Parameters
|Name|Type|Description|
|---|---|---|
|str|DYNARRAY[] of CHAR|Source string.|

## Examples
```pascal
revisedString := 'vectorworks';

UprString(revisedString);

{Sets revisedString equal to 'VECTORWORKS'}
```

## Version
Availability: from MiniCAD
## Category
* Strings

