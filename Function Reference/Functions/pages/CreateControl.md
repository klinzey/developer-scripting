# CreateControl

## Description
Creates a new extended dialog control item. Supported extended dialog controls include image, system color palette, and slider controls.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Control Types&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
        &lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
          &lt;TR BGCOLOR=#000000&gt; 
            &lt;TH&gt; &lt;CENTER&gt;
                &lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
            &lt;TH&gt; &lt;CENTER&gt;
                &lt;FONT COLOR=#FFFFFF&gt;Control Type&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
          &lt;/TR&gt;
          &lt;TR&gt; 
            &lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
                1 &lt;/CENTER&gt;&lt;/TD&gt;
            &lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
                Image &lt;/CENTER&gt;&lt;/TD&gt;
          &lt;/TR&gt;
          &lt;TR&gt; 
            &lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
                2 &lt;/CENTER&gt;&lt;/TD&gt;
            &lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
                System Color &lt;/CENTER&gt;&lt;/TD&gt;
          &lt;/TR&gt;
          &lt;TR&gt; 
            &lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
                3 &lt;/CENTER&gt;&lt;/TD&gt;
            &lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
                Slider &lt;/CENTER&gt;&lt;/TD&gt;
          &lt;/TR&gt;
          &lt;TR&gt; 
            &lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
                10 &lt;/CENTER&gt;&lt;/TD&gt;
            &lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
                Image Popup &lt;/CENTER&gt;&lt;/TD&gt;
          &lt;/TR&gt;
          &lt;TR&gt; 
            &lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
                11 &lt;/CENTER&gt;&lt;/TD&gt;
            &lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
                Gradient Slider &lt;/CENTER&gt;&lt;/TD&gt;
          &lt;/TR&gt;
        &lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE CreateControl(
				dialogID    : LONGINT;
				itemID      : LONGINT;
				controlKind : LONGINT;
				name        : STRING;
				data        : LONGINT);
```

```python

def vs.CreateControl(dialogID, itemID, controlKind, name, data):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|controlKind|LONGINT|The type of control item.|
|name|STRING|The display text of the control item.|
|data|LONGINT|Initial data for the control item.|

## Remarks
[DWD 1/20/00]

## Examples
```pascal
{open the resource file containing the graphics for the dialog}

rsAvailable:= SetVSResourceFile('Images');

{creates a new image control}

 CreateControl(lEditID,5,1,'SplashImage',1010);



{Slider Control Example}

PROCEDURE dialog1_Main;

CONST

	kSlider = 4;

	kLabel  = 5;

	kValue  = 6;

VAR

	dialog1   :INTEGER;

	gSlider   :LONGINT;



PROCEDURE dialog1_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

	CASE item OF

		kSlider:

			BEGIN

				GetControlData(dialog1, kSlider, gSlider);

				SetField(kValue, Concat(gSlider));

			END;

	END;

END;



BEGIN

	gSlider := 1000;

	dialog1 := CreateLayout('Slider Control', False, 'OK', 'Cancel');

	CreateControl     (dialog1, kSlider,  3, '', 1000);

	CreateStaticText  (dialog1, kLabel,   'Slider Value:', -1);

	CreateStaticText  (dialog1, kValue,   ' ', -1);

	SetFirstLayoutItem(dialog1, kSlider);

	SetBelowItem      (dialog1, kSlider,  kLabel,   0, 0);

	SetRightItem      (dialog1, kLabel,   kValue,   0, 0);

	IF RunLayoutDialog(dialog1, dialog1_Handler) = 1 THEN BEGIN

	END;

END;

RUN(dialog1_Main);


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern

