# AddSymToWallEdge

## Description
Procedure AddSymToWallEdge inserts a symbol in the referenced wall using the specified parameters to define placement. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Symbol Insertion Alignment&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Alignment&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Centerline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Left Edge&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Right Edge&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE AddSymToWallEdge(
				h              : HANDLE;
				alongDistance  : REAL (Coordinate);
				heightDistance : REAL (Coordinate);
				flip           : BOOLEAN;
				right          : BOOLEAN;
				symbolName     : STRING;
				insertMode     : INTEGER);
```

```python

def vs.AddSymToWallEdge(h, alongDistance, heightDistance, flip, right, symbolName, insertMode):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to wall.|
|alongDistance|REAL (Coordinate)|Offset distance from wall start of insertion point.|
|heightDistance|REAL (Coordinate)|Elevation of symbol.|
|flip|BOOLEAN|Flip orientation of symbol.|
|right|BOOLEAN|Left-right orientation of symbol.|
|symbolName|STRING|Name of symbol to be inserted.|
|insertMode|INTEGER|Edge insertion mode.|

## Remarks
Inserts a symbol in a wall either on the centerline, or on the edge. All parameters are used as input.<BR>
<BR>
h = handle to the wall we are inserting into.<BR>
alongDistance = distance along the wall from the wall starting point to the symbols insertion point.<BR>
heightDistance = height of the symbol in 3D<BR>
flip = sets the orientation<BR>
right = sets the orientaion<BR>
symbolName = the name of master symbol that gets inserted in the wall<BR>
insertMode = 0 for centerline, 1 for left edge, 2 for right edge<BR>
[sd 8/18/98]

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Walls

