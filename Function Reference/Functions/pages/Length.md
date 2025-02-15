# Length

## Description
Returns the length of an object. If more than one object matches the search criteria, the function will return the sum of all the matching object lengths.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Length(c : CRITERIA) : REAL;
```

```python

def vs.Length(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
LengthValue:=Length(C='CrossMembers');

{returns the length of all objects in class 'CrossMembers'}
```

## Version
```diff
- Length is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria

