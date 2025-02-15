# BeginFloor

## Description
Procedure BeginFloor creates a new floor object in a Vectorworks document. BeginFloor uses 2D object creation procedure calls to define the &amp;quot;template&amp;quot; for the object. &lt;BR&gt;
&lt;BR&gt;
After specifying object procedure calls to define the floor object, you should call EndGroup to complete the column definition and create the actual object.&lt;BR&gt;


```pascal
PROCEDURE BeginFloor(thicknessDistance : REAL (Coordinate));
```

```python

def vs.BeginFloor(thicknessDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|thicknessDistance|REAL (Coordinate)|Floor thickness.|

## Examples
```pascal
BeginFloor(6&quot;);

Rect(1,1,5,5);

EndGroup;
```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Architectural

