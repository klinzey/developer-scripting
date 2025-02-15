# Pos

## Description
Function Pos searches for a specified substring contained within in a target string.&lt;BR&gt;
&lt;BR&gt;
Pos returns the position of the substring. If the string is not found, 0 is returned.&lt;BR&gt;


```pascal
FUNCTION Pos(
				subStr : DYNARRAY[] of CHAR;
				str    : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.Pos(subStr, str):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|subStr|DYNARRAY[] of CHAR|Substring to be located.|
|str|DYNARRAY[] of CHAR|Target string.|

## Examples
```pascal
Loc:=Pos('samp','A sample string');


```

## Version
Availability: from MiniCAD
## Category
* Strings

