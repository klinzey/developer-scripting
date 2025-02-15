# AddCavity

## Description
Procedure AddCavity creates a wall cavity in a new wall object. The newly defined cavity becomes the default for all subsequently defined walls.&lt;BR&gt;
&lt;BR&gt;
To apply a bitmap fill pattern, use positive value corresponding to the index  of the bitmap pattern.  To apply a vector fill pattern, use the negative of the vector fill index (index * -1). &lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.


```pascal
PROCEDURE AddCavity(
				pair             : BOOLEAN;
				leftOffDistance  : REAL (Coordinate);
				rightOffDistance : REAL (Coordinate);
				pairFill         : LONGINT);
```

```python

def vs.AddCavity(pair, leftOffDistance, rightOffDistance, pairFill):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|pair|BOOLEAN|Double line display mode.|
|leftOffDistance|REAL (Coordinate)|Left edge offset from wall centerline.|
|rightOffDistance|REAL (Coordinate)|Right edge offset from wall centerline.|
|pairFill|LONGINT|Fill index for filled cavities.|

## Remarks
OBSOLETE for Version 12: This function is obsolete. Use InsertNewComponent instead. (NZH 5-9-05)

## Examples
```pascal
{ Create wall object with 1&quot; wide cavity using black pattern fill.}

DoubLines(6&quot;);

AddCavity(True, 1&quot;, 2&quot;, 2);

Wall(0, 1, 9, 1);



{ Create wall object with 1&quot; wide cavity using a custom hatch fill.}

DoubLines(6&quot;);

AddCavity(True, 1&quot;, 2&quot;, -Name2Index('My Hatch'));

Wall(0, 1, 9, 1);


```

## Version
```diff
- AddCavity is obsolete as of VectorWorks12.0
```

Availability: from MiniCAD4.0
## Category
* Objects - Walls

