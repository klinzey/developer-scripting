# GetLightFalloff

## Description
Procedure GetLightFalloff returns the fall off attributes for the referenced light object. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Light Falloff Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Falloff Type&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;None&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Normal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Smooth&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Sharp&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE GetLightFalloff(
				light           : HANDLE;
				VAR distFalloff : INTEGER;
				VAR angFalloff  : INTEGER);
```

```python

def vs.GetLightFalloff(light):
    return (distFalloff, angFalloff)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|light|HANDLE|Handle to light.|
|distFalloff|INTEGER|Returns distance falloff value.|
|angFalloff|INTEGER|Returns angular falloff value.|

## Remarks
Returns the falloff functions for the light.  0 = None, 1 = Normal, 2 = Smooth, 3 = Sharp (angular falloff only).

## Version
Availability: from MiniCAD7.0.1
## Category
* Objects - Lights

