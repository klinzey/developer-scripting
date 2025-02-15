# CopyMode

## Description
Procedure CopyMode sets the transfer mode for the active design layer.  If a sheet layer is active, the procedure has no effect.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Transfer Modes&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Transfer Mode&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Index Value&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Copy&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;8&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;OR&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;9&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;XOR&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;10&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;BIC&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;11&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Inverse Copy&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;12&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Inverse OR&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;13&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Inverse XOR&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;14&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Inverse BIC&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;15&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
The design layer will only be imaged with the transfer mode on systems which support it, like Windows.  Setting the transfer mode to a mode other than Copy (i.e. 8, Paint mode), when the current layer transparency percentage is 0, will also automatically change the layer transparency percentage to 50.  Similarly, setting the transfer mode to Copy, when the current layer transparency percentage is greater than 0, will also automatically change the layer transparency percentage to 0.  This is to approximately preserve the appearance of the layer on systems that don't support transfer modes, like Quartz on the Mac.&lt;BR&gt;


```pascal
PROCEDURE CopyMode(mode : INTEGER);
```

```python

def vs.CopyMode(mode):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|mode|INTEGER|Mode index value.|

## Remarks
Sets the layer transfer mode for the actlve layer.<BR>
<BR>
Valid mode values are:<BR>
8 - Copy<BR>
9 - OR<BR>
10 - XOR<BR>
11 - BIC<BR>
12 - Inverse Copy<BR>
13 - Inverse OR<BR>
14 - Inverse XOR<BR>
15 - Inverse BIC<BR>
<BR>
This procedure may also set the layer transparency to approximate the given transfer mode on systems that don't support transfer modes.

## See Also
VS Functions:
[SetLayerTransparency](SetLayerTransparency.md)

## Version
Availability: from MiniCAD
## Category
* Layers

