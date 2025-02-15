# BeginColumn

## Description
Procedure BeginColumn creates a column object in a Vectorworks document using 2D object creation procedure calls to define the &amp;quot;template&amp;quot; for the column object. &lt;BR&gt;
&lt;BR&gt;
After specifying object procedure calls to define the column, you should call EndGroup to complete the column definition and create the actual object.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE BeginColumn(columnDistance : REAL (Coordinate));
```

```python

def vs.BeginColumn(columnDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|columnDistance|REAL (Coordinate)|Height of column.|

## Remarks
BeginColumn takes the group of objects that follow, until there is an EndGroup, and converts them into a column with height equal to column distance.<BR>
<BR>
[sd 8/17/98]

## Examples
```pascal
BeginColumn(12');

  Oval(2',2',6',6');

EndGroup;
```

## Version
Availability: from MiniCAD7.0
## Category
* Objects - Architectural

