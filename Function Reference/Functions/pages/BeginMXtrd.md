# BeginMXtrd

## Description
Procedure BeginMXtrd creates a multiple extrude object in a Vectorworks document. BeginMXtrd uses 2D object creation procedure calls to define the &amp;quot;template&amp;quot; for the object.&lt;BR&gt;
&lt;BR&gt;
You should call EndMXtrd after the object creation procedures to complete the definition and generate the object in the document.&lt;BR&gt;
&lt;BR&gt;
A multiple extrude object is a 3D object created from three or more 2D objects, which are used as defining shapes for the extruded object.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE BeginMXtrd(
				startDistance : REAL (Coordinate);
				endDistance   : REAL (Coordinate));
```

```python

def vs.BeginMXtrd(startDistance, endDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startDistance|REAL (Coordinate)|Start distance from document ground plane.|
|endDistance|REAL (Coordinate)|End distance from document ground plane.|

## Examples
```pascal
BeginMXtrd(0',1 363/512&quot;);

  Rect(-125/128&quot;,1 113/512&quot;,375/512&quot;,375/512&quot;);

  Rect(-25/32&quot;,1 113/512&quot;,275/512&quot;,375/512&quot;);

  Rect(-75/128&quot;,1 113/512&quot;,325/1024&quot;,375/512&quot;);

  Locus(-275/2048&quot;,125/128&quot;);

  Rect(-75/128&quot;,1 113/512&quot;,325/1024&quot;,375/512&quot;);

  Rect(-25/32&quot;,1 113/512&quot;,275/512&quot;,375/512&quot;);

  Rect(-125/128&quot;,1 113/512&quot;,375/512&quot;,375/512&quot;);

EndMXtrd;


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D

