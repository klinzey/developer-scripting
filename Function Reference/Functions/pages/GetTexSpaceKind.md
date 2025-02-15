# GetTexSpaceKind

## Description
Function GetTexSpaceKind returns the object type for texture mapping space.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Texture Mapping Spaces&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Date Style&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plane&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Sphere&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Cylinder&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Algorithmic&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION GetTexSpaceKind(textureSpace : HANDLE) : INTEGER;
```

```python

def vs.GetTexSpaceKind(textureSpace):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|

## Remarks
Returns the kind of the texture mapping space; 0 = Plane space, 1 = Sphere, 2 = Cylinder, and 3 = Algorithmic (Perimeter or Roof)

## Version
```diff
- GetTexSpaceKind is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures

