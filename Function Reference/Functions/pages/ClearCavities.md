# ClearCavities

## Description
Procedure ClearCavities resets the default cavity style of wall objects to no cavities.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE ClearCavities;
```

```python

def vs.ClearCavities():
    return None
```

## Examples
```pascal
DoubLines(6&quot;);

AddCavity(True,1&quot;,2&quot;,2);

Wall(0,1,9,1);

ClearCavities;

Wall(0,2,11,2);

{creates a wall with a cavity, then creates a wall without a cavity}
```

## Version
```diff
- ClearCavities is obsolete as of VectorWorks12.5
```

Availability: from MiniCAD4.0
## Category
* Objects - Walls

