# SetTextVerticalAlign

## Description
Procedure SetTextVerticalAlign sets the vertical alignment of the referenced text object. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Text Vertical Justification&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Justification&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top of text box&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Top baseline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Text centerline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bottom baseline&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bottom of text box&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/textlocus.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;

```pascal
PROCEDURE SetTextVerticalAlign(
				TextHd            : HANDLE;
				verticalAlignment : INTEGER);
```

```python

def vs.SetTextVerticalAlign(TextHd, verticalAlignment):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|TextHd|HANDLE|Handle to text object.|
|verticalAlignment|INTEGER|Vertical alignment setting for text.|

## Remarks
Sets the vertical alignment of the referenced text object.

## See Also
VS Functions:
[SetTextVertAlignN](SetTextVertAlignN.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text

