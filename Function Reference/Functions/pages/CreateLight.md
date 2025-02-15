# CreateLight

## Description
CreateLight creates a new light object in the active VectorScript document. &lt;BR&gt;
&lt;BR&gt;
A new light objects' color is defaulted to white, and brightness is defaulted to 75%. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Light Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Light Type&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Directional&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Point&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Spot&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION CreateLight(
				pXR        : REAL;
				pYR        : REAL;
				pZR        : REAL;
				lightType  : INTEGER;
				isOn       : BOOLEAN;
				castShadow : BOOLEAN) : HANDLE;
```

```python

def vs.CreateLight(pXR, pYR, pZR, lightType, isOn, castShadow):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|pXR|REAL|X coordinate of new light.|
|pYR|REAL|Y coordinate of new light.|
|pZR|REAL|Z coordinate of new light.|
|lightType|INTEGER|Light type.|
|isOn|BOOLEAN|On-off status of light.|
|castShadow|BOOLEAN|Specifies whether light will cast shadow.|

## Examples
```pascal
CreateLight(2,3,8,1,TRUE,TRUE);


```

## Version
Availability: from MiniCAD7.0
## Category
* Objects - Lights

