# GetLVis

## Description
Function GetLVis returns the visibility of the referenced layer.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Layer Visibility&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Visibility&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Index Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Normal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Grayed&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Invisible&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;-1&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;


```pascal
FUNCTION GetLVis(h : HANDLE) : INTEGER;
```

```python

def vs.GetLVis(h):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to layer.|

## Examples
```pascal
FUNCTION GetLayerVisibility(layerHandle :handle) :INTEGER;

	{Returns the effective visibility of a layer.}

BEGIN

	GetLayerVisibility := -1;

	IF layerHandle = ActLayer THEN GetLayerVisibility := 0 ELSE {Active layers are always visible.}

	IF (GetObjectVariableInt(ActLayer, 154) = 1) &amp; (GetObjectVariableInt(layerHandle, 154) = 1) THEN BEGIN

		{If it's not the active layer, then the only way that it can be visible is if

		the active layer is a design layer, and so is layerHandle, and the combination

		of layer options and the layer's visibility will result in a visible layer.}

		IF (GetLayerOptions = 2) &amp; (GetLVis(layerHandle) = 2) THEN GetLayerVisibility := 2 ELSE

		IF (GetLayerOptions = 2) &amp; (GetLVis(layerHandle) = 0) THEN GetLayerVisibility := 2 ELSE

		IF (GetLayerOptions &gt; 2) &amp; (GetLVis(layerHandle) = 2) THEN GetLayerVisibility := 2 ELSE

		IF (GetLayerOptions &gt; 2) &amp; (GetLVis(layerHandle) = 0) THEN GetLayerVisibility := 0;

	END;

END;





PROCEDURE Example;

BEGIN

	Message(GetLVis(GetLayerByName('Layer-1')));

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Layers

