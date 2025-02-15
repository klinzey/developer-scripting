# CreateEditReal

## Description
Creates an editable text field control for REAL values.&lt;BR&gt;
&lt;BR&gt;
CreateEditReal is intended specifically for entry of numeric values; the control returns values in a numeric format, and supports calculations within the control field.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Field Types for EditReal Fields&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Index &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Field Value &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		1  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		REAL value  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		2  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Angular value  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		3  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Dimension  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		4  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		X coordinate  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		5  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Y coordinate  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;


```pascal
PROCEDURE CreateEditReal(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				editRealType   : LONGINT;
				defaultValue   : REAL;
				widthInStdChar : LONGINT);
```

```python

def vs.CreateEditReal(dialogID, itemID, editRealType, defaultValue, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|editRealType|LONGINT|The type of REAL value being accepted.|
|defaultValue|REAL|Default value for the field.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Remarks
Edits reals, does math,  get and set values with get and set real calls. There are 5 edit real types: 1 - Real, regular old real type; 2 - Angle, vs input and output is always in degrees but the user can use what ever they want; 3 - Dimension, usually an offset this a distance that is not tied to the origin; 4 - 4- CoordinateX, this is an exact x location on the drawing; 5-CoordinateY, this is an exact y location on the drawing. There are separate x and y controls to account for changes the user may make to the origin. I think Z coordinates should use the offset mode, but I need to check with mark on this one.  Darick

## Examples
```pascal
PROCEDURE Example;

VAR

	dialog1 :INTEGER;

	result  :INTEGER;

PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

END;

BEGIN

	dialog1 := CreateLayout('Example Dialog', FALSE, 'OK', 'Cancel');

	CreateEditReal(dialog1, 4, 3, 123, 16);

	SetFirstLayoutItem(dialog1, 4);

	result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern

