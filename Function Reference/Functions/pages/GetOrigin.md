# GetOrigin

## Description
Procedure GetOrigin returns the current origin location relative to the center of the page.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE GetOrigin(
				VAR x : REAL;
				VAR y : REAL);
```

```python

def vs.GetOrigin():
    return (x, y)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|x|REAL|Returns X coordinate of origin.|
|y|REAL|Returns Y coordinate of origin.|

## Examples
```pascal
PROCEDURE Example;

VAR

   originPt :VECTOR;

BEGIN

   GetOrigin(originPt.x, originPt.y);

   Message(originPt);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Document Settings

