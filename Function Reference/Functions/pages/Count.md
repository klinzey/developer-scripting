# Count

## Description
Counts all of the objects which match the search criteria.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Count(c : CRITERIA) : LONGINT;
```

```python

def vs.Count(c):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
CountValue := Count((FP=4)and(T='Rect'));

{counts all rectangles with a fillpat index of 4}
```

## Version
Availability: from MiniCAD
## Category
* Criteria

