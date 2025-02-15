# Delete

## Description
Procedure Delete removes a substring from the specified source string.&lt;BR&gt;


```pascal
PROCEDURE Delete(
				VAR source : DYNARRAY[] of CHAR;
				index      : INTEGER;
				count      : INTEGER);
```

```python

def vs.Delete(source, index, count):
    return source
```

## Parameters
|Name|Type|Description|
|---|---|---|
|source|DYNARRAY[] of CHAR|Source string.|
|index|INTEGER|Start position in text string.|
|count|INTEGER|Length of substring.|

## Examples
```pascal
theStr:='A sample string';

Delete(theStr,3,7);

{deletes 'sample' from the string value}
```

## Version
Availability: from MiniCAD
## Category
* Strings

