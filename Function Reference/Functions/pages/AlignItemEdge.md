# AlignItemEdge

## Description
Aligns the specified control item with other items having the same edge and alignment id values. To align several control items, call this function once for each item to be aligned using a common alignment id value.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Alignment Options&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Alignment Edge&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		1 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Right &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		2 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Bottom &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		3 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Left &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt;Alignment Mode&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		0 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;Resize control items&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		1 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#000000&gt;Shift control items&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;
Right alignment of objects will use the object with the minimum pixel value as the alignment baseline. Bottom and left alignment of objects will use the object with the  maximum pixel value as the alignment baseline.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE AlignItemEdge(
				dialogID  : LONGINT;
				itemID    : LONGINT;
				whichEdge : LONGINT;
				alignID   : INTEGER;
				alignMode : INTEGER);
```

```python

def vs.AlignItemEdge(dialogID, itemID, whichEdge, alignID, alignMode):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout being defined.|
|itemID|LONGINT|The index of the control item to be aligned.|
|whichEdge|LONGINT|The control edge to be aligned.|
|alignID|INTEGER|An arbitrary number used to identify the items to be aligned together.|
|alignMode|INTEGER|Alignment mode of the operation|

## Remarks
Aligns layout items with the same edge and alignID. whichEdge: 1=right, 2=bottom, 3=left; alignMode: resize=0, shift=1<BR>
<BR>
Right aligned objects are lined up with the object with the minimum pixel value. Bottom and left aligned objects are lined up on the maximum pixel value.[DWD 1/20/00]

## Examples
```pascal
{aligns all items with the positioning ID of 99}

	AlignItemEdge(lEditID,4,1,99,0);

	AlignItemEdge(lEditID,6,1,99,0);


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern

