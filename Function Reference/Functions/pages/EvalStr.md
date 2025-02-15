# EvalStr

## Description
Evaluates whether an object meets the specified search criteria. &lt;BR&gt;
&lt;BR&gt;
When used with record criteria, it will determine whether a specific record is attached to the object; if used with record-field criteria, it will return the value of the field as a STRING.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION EvalStr(
				h : HANDLE;
				c : CRITERIA) : STRING;
```

```python

def vs.EvalStr(h, c):
    return STRING
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
dataValue:= EvalStr(handleToObject,('Part Info'.'Serial No.'));
```

## Version
Availability: from MiniCAD
## Category
* Criteria

