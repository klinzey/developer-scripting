# Marker

## Description
Marker defines a marker (arrowhead) style for the document. This marker style becomes the active style for the document.&lt;BR&gt;
&lt;BR&gt;
A complete listing of marker styles can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#marker&quot;&gt;Appendix&lt;/A&gt;


```pascal
PROCEDURE Marker(
				style : INTEGER;
				size  : REAL;
				ang   : INTEGER);
```

```python

def vs.Marker(style, size, ang):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|style|INTEGER|Marker style constant.|
|size|REAL|Marker size in inches measured in page space.  Legal values are 0.0 to 2.0.|
|ang|INTEGER|Marker angle.|

## Remarks
OBSOLETE for VW2008: Use SetDefaultBeginningMarker and/or SetDefaultEndMarker instead.<BR>
See FMarker for parameter descriptions.<BR>
<BR>
[sd 8/14/98]

## Examples
```pascal
Marker(2,0.25,60);


```

## Version
```diff
- Marker is obsolete as of VectorWorks 2008
```

Availability: from MiniCAD6.0
## Category
* Document Attributes

