# ResolveByClassTextureRef

## Description
Function ResolveByClassTextureRef returns the internal index, or name, of the texture assigned to the referenced object. &lt;BR&gt;
&lt;BR&gt;
Primary, secondary, or tertiary texture assignments can be returned for objects that support multiple textures, such as roofs or walls. For objects that do not support multiple textures, pass 0 to the partID parameter.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Object Texture Reference&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Texture&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Index Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Primary&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Secondary&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Tertiary&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION ResolveByClassTextureRef(
				obj    : HANDLE;
				partID : INTEGER) : LONGINT;
```

```python

def vs.ResolveByClassTextureRef(obj, partID):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|partID|INTEGER|Primary, secondary, or tertiary texture ID to be returned.|

## Remarks
If the texture ref for an object is set to -1, it will use the texture of its class.  This routine will look up the object's class and return the class' texture ref.

## Examples
```pascal
textureID:=ResolveByClassTextureRef(handleToObject,0);
```

## See Also
VS Functions:
[SetTextureRef](SetTextureRef.md)| [GetTextureRef](GetTextureRef.md)

## Version
Availability: from VectorWorks8.0
## Category
* Textures

