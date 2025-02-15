# BeginSweep

## Description
Procedure BeginSweep creates a three-dimensional sweep object in the Vectorworks document. A sweep object is a two-dimensional template object which has been rotated about a specified point to create a 3D object. For example, a circle of radius 1&amp;quot; that is swept about a point 2&amp;quot; to the right of the circles center wil create a sweep object resembling a donut, also known as a torus.&lt;BR&gt;
&lt;BR&gt;
The sweep increment may also be thought of as the spacing between the duplication of radial sweep mesh lines. The &amp;quot;pitch&amp;quot;, or vertical distance, is the distance that the sweep object will travel for every 360° of rotation.  In sweep objects, the 2D template object may also be translated as it rotates, resulting in a &amp;quot;corkscrew&amp;quot; effect. The vertical movement is determined by the following equation: vertical movement = pitch * ArcAngle/360.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt; 2D Object &quot;Template&quot; for Sweep&lt;/I&gt;&lt;P&gt;&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/sweep2d.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;&lt;BR&gt;
&lt;I&gt; Sweep Object&lt;/I&gt;&lt;P&gt;&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/sweep3d.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;

```pascal
PROCEDURE BeginSweep(
				startAngle    : REAL;
				arcAngle      : REAL;
				incAngle      : REAL;
				PitchDistance : REAL (Coordinate));
```

```python

def vs.BeginSweep(startAngle, arcAngle, incAngle, PitchDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startAngle|REAL|Starting angle of the sweep.|
|arcAngle|REAL|Angle of sweep.|
|incAngle|REAL|Increment of sweep.|
|PitchDistance|REAL (Coordinate)|Pitch (translation distance) of sweep.|

## Examples
```pascal
BeginSweep(#0d,#360d,#10d,0');

  Poly(3 1/4&quot;,-1/2&quot;,

       3 1/4&quot;,-1&quot;,

       2 3/4&quot;,-1&quot;,

       2 1/4&quot;,-1/2&quot;,

       2 1/4&quot;,1&quot;,

       1 3/4&quot;,1 1/2&quot;,

       -1 3/4&quot;,1 1/2&quot;,

       -2 1/4&quot;,1&quot;,

       -2 1/4&quot;,-1/2&quot;,

       -2 3/4&quot;,-1&quot;,

       -3 1/4&quot;,-1&quot;,

       -3 1/4&quot;,-1/2&quot;,

       -2 3/4&quot;,0&quot;,

       -2 3/4&quot;,1 1/2&quot;,

       -2 1/4&quot;,2&quot;,

       2 1/4&quot;,2&quot;,

       2 3/4&quot;,1 1/2&quot;,

       2 3/4&quot;,0&quot;);

EndSweep;


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D

