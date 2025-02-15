# ForEachObject

## Description
Calls a user defined procedure to operate on each object matching the specified search criteria. &lt;BR&gt;
&lt;BR&gt;
The procedure subroutine specified by the callback parameter must have one parameter of type HANDLE, which is passed the handle to an object by the ForEachObject call.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE ForEachObject(
				callback : PROCEDURE;
				c        : CRITERIA);
```

```python

def vs.ForEachObject(callback, c):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|callback|PROCEDURE|Name of action procedure to be applied to matching objects|
|c|CRITERIA|Search criteria for locating objects.|

## Examples
```pascal
PROCEDURE PickRect;



PROCEDURE SelectThem(h :HANDLE);

BEGIN

	SetSelect(h);

END;



BEGIN

	ForEachObject(SelectThem, T=RECT);

END;

RUN(PickRect);


```

## Version
Availability: from MiniCAD
## Category
* Criteria

