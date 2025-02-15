# GetPt

## Description
Procedure GetPt switches the cursor to selection mode and allows the user to select a point in a Vectorworks document. This cannot be used if there is a function anywhere in the calling chain.&lt;BR&gt;


```pascal
PROCEDURE GetPt(VAR p : REAL);
```

```python

def vs.GetPt():
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Returns coordinates of mouse click.|

## Examples
```pascal
PROCEDURE Example;

VAR

	pt :POINT;

BEGIN

	GetPt(pt.x, pt.y);

	Message(pt);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* User Interactive

