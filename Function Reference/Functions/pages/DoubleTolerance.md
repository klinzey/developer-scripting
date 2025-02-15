# DoubleTolerance

## Description
Procedure DoubleTolerance is used with dimensioning procedures to define a tolerance for the most recently created dimension.&lt;BR&gt;


```pascal
PROCEDURE DoubleTolerance(
				showVal     : BOOLEAN;
				boxText     : BOOLEAN;
				leader      : STRING;
				trailer     : STRING;
				topDistance : REAL (Coordinate);
				botDistance : REAL (Coordinate));
```

```python

def vs.DoubleTolerance(showVal, boxText, leader, trailer, topDistance, botDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|showVal|BOOLEAN|Dimension text display flag.|
|boxText|BOOLEAN|Boxed text display flag.|
|leader|STRING|Dimension leader text string.|
|trailer|STRING|Dimension trailer text string.|
|topDistance|REAL (Coordinate)|Tolerance value text string.|
|botDistance|REAL (Coordinate)|Tolerance value text string.|

## Examples
```pascal
LinearDim(-2&quot;,2&quot;,1&quot;,2&quot;,-3&quot;,0,771,771,0.75);

DoubleTolerance(True,False,'est. ','',1/16&quot;,1/16&quot;);

{defines a dimension with a double tolerance}
```

## Version
Availability: from MiniCAD4.0
## Category
* Dimensions

