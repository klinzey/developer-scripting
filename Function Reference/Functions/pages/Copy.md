# Copy

## Description
Function Copy returns a substring from a specified source string.&lt;BR&gt;


```pascal
FUNCTION Copy(
				source : DYNARRAY[] of CHAR;
				index  : INTEGER;
				count  : INTEGER) : DYNARRAY[] of CHAR;
```

```python

def vs.Copy(source, index, count):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|source|DYNARRAY[] of CHAR|Source string.|
|index|INTEGER|Start position in text string.|
|count|INTEGER|Length of substring.|

## Examples
```pascal
newStr:=Copy('A sample string',10,6);

{returns 'string'}


```

## Version
Availability: from MiniCAD
## Category
* Strings

