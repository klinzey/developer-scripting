# Eval

## Description
Evaluates whether an object meets the specified search criteria. &lt;BR&gt;
&lt;BR&gt;
When used with record criteria, it will determine whether a specific record is attached to the object; if used with record-field criteria, it will return the value of the field as a REAL value.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Eval(
				h : HANDLE;
				c : CRITERIA) : REAL;
```

```python

def vs.Eval(h, c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle of object to which the search criteria will be applied.|
|c|CRITERIA|Search criteria.|

## Returns
If the criteria is a record-field criteria, the procedure will return the value contained within the field. All other criteria return the TRUE-FALSE state of the criteria condition. 

## Examples
```pascal
hasRecord:=Eval(handleToObject,(R IN ['Part Info']);
```

## Version
Availability: from MiniCAD
## Category
* Criteria

