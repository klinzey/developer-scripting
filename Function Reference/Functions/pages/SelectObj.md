# SelectObj

## Description
Selects all objects which match the search criteria.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SelectObj(c : CRITERIA);
```

```python

def vs.SelectObj(c):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
PROCEDURE Example;

VAR

	red, green, blue, color :LONGINT;

	criteria :STRING;

BEGIN

	red := 65535;

	green := 0;

	blue := 0;

	RGBToColorIndex(red, green, blue, color);

	Rect(0, 0, 1, 1);

	SetPenFore(LNewObj, color);

	DSelectAll;

	criteria := Concat('(INSYMBOL &amp; INVIEWPORT &amp; (PF=', color, '))');

	SelectObj(criteria);

	Message(criteria);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Criteria

