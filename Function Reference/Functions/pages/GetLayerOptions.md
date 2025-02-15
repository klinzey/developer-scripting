# GetLayerOptions

## Description
Returns layer visibility setting for the active document.&lt;BR&gt;
&lt;BR&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Visibility&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Active Only&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Gray Others&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Gray/Snap Others&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Show Others&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Show/Snap Others&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Show/Snap/Modify Others&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION GetLayerOptions : INTEGER;
```

```python

def vs.GetLayerOptions():
    return INTEGER
```

## Returns
Returns an INTEGER indicating the layer visibility status of the document.

## See Also
VS Functions:
[SetLayerOptions](SetLayerOptions.md)

## Version
Availability: from VectorWorks8.5
## Category
* Layers

