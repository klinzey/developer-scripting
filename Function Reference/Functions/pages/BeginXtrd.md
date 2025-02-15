# BeginXtrd

## Description
Procedure BeginXtrd creates a 3D extrude object in a Vectorworks document. BeginXtrd uses 2D object creation procedure calls to define the &amp;quot;template&amp;quot; for the object. &lt;BR&gt;
&lt;BR&gt;
You should call EndXtrd after the object creation procedures to complete the definition and generate the extrude object in the document.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE BeginXtrd(
				startDistance : REAL (Coordinate);
				endDistance   : REAL (Coordinate));
```

```python

def vs.BeginXtrd(startDistance, endDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startDistance|REAL (Coordinate)|Start distance from document ground plane.|
|endDistance|REAL (Coordinate)|End distance from document ground plane.|

## Examples
```pascal
BeginXtrd(0',4');

Rect(-1 61/64&quot;,125/128&quot;,-1 119/256&quot;,-375/512&quot;);

Rect(-1 113/512&quot;,1 113/512&quot;,-375/512&quot;,-125/256&quot;);

Rect(-125/256&quot;,125/128&quot;,0',-375/512&quot;);

Rect(125/128&quot;,125/128&quot;,1 119/256&quot;,-375/512&quot;);

Rect(1 25/512&quot;,1 113/512&quot;,375/512&quot;,-125/256&quot;);

Rect(1 363/512&quot;,1 113/512&quot;,2 101/512&quot;,-125/256&quot;);

EndXtrd;

{creates an extrude using the defined rectangles, each extruded to a depth of 4'}
```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D

