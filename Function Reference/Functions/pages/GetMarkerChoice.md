# GetMarkerChoice

## Description
OBSOLETE procedure for VW2008&lt;BR&gt;
Get current choice for Marker popup dialog control.

```pascal
PROCEDURE GetMarkerChoice(
				dialogID  : LONGINT;
				itemID    : LONGINT;
				VAR index : INTEGER;
				VAR style : INTEGER;
				VAR angle : INTEGER;
				VAR size  : REAL);
```

```python

def vs.GetMarkerChoice(dialogID, itemID):
    return (index, style, angle, size)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|index|INTEGER||
|style|INTEGER||
|angle|INTEGER||
|size|REAL||

## Examples
```pascal
PROCEDURE Example;

VAR

   int, dialogID   :INTEGER;

   index, style, angle :INTEGER;

   size :REAL;



PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

   CASE item OF

      SetupDialogC:

         BEGIN

            index := 1;

            style := 2;

            angle := 3;

            size  := .125;

            SetMarkerChoice(dialogID, 4, index, style, angle, size);

         END;

      5: 

         BEGIN

            GetMarkerChoice(dialogID, 4, index, style, angle, size);

            AlrtDialog(Concat(

	            'index: ', index, Chr(13), 

	            'style: ', style, Chr(13), 

	            'angle: ', angle, Chr(13), 

	            'size: ', size));

         END;

   END;

END;



BEGIN

   dialogID := CreateLayout('Test', False, 'OK', '');

   CreateMarkerPopup(dialogID, 4);

   CreatePushButton(dialogID, 5, '  Display Values  ');

   SetFirstLayoutItem(dialogID, 4);

   SetBelowItem(dialogID, 4, 5, 0, 2);

   int := RunLayoutDialog(dialogID, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[SetMarkerChoice](SetMarkerChoice.md)

## Version
```diff
- GetMarkerChoice is obsolete as of VectorWorks 2008
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern

