# GetLightInfo

## Description
Procedure GetLightInfo returns the attributes of the referenced light object.&lt;BR&gt;
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
&lt;/CENTER&gt;

```pascal
PROCEDURE GetLightInfo(
				h              : HANDLE;
				VAR lightType  : INTEGER;
				VAR brightness : INTEGER;
				VAR isOn       : BOOLEAN;
				VAR castShadow : BOOLEAN);
```

```python

def vs.GetLightInfo(h):
    return (lightType, brightness, isOn, castShadow)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to light.|
|lightType|INTEGER|Returns light type.|
|brightness|INTEGER|Returns light brightness.|
|isOn|BOOLEAN|Returns on-off status of light.|
|castShadow|BOOLEAN|Returns whether light casts shadows.|

## Version
Availability: from MiniCAD7.0
## Category
* Objects - Lights

