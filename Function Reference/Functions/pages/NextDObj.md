# NextDObj

## Description
Function NextDObj returns the next deselected object after the referenced object in a list. If the end of the list is reached, the function returns NIL.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION NextDObj(h : HANDLE) : HANDLE;
```

```python

def vs.NextDObj(h):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
handleToObject:=FObject;

WHILE handleToObject &lt;&gt; NIL DO BEGIN

  SetSelect(handleToObject);

  handleToObject:=NextDObj(handleToObject);

END;

{ selects all deselected objects }


```

## Version
Availability: from MiniCAD
## Category
* Document List Handling

