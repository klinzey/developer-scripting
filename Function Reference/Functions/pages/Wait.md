# Wait

## Description
Procedure Wait delays execution in VectorScript for a specified number of seconds.&lt;BR&gt;
&lt;BR&gt;
When paused, a VectorScript routine stops at the point where Wait is encountered.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Wait(seconds : INTEGER);
```

```python

def vs.Wait(seconds):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|seconds|INTEGER|Number of seconds to pause script execution.|

## Examples
```pascal
Wait(3);

{pauses execution for 3 seconds}
```

## Version
Availability: from MiniCAD
## Category
* Utility

