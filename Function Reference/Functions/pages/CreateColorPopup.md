# CreateColorPopup

## Description
Create a color popup dialog control that displays the 256 color palette associated with the active document.  &lt;BR&gt;
&lt;BR&gt;
The widthInStdChar argument specifies the width of the control.  Pass -1 to request the default size, which will be consistent with other attribute controls (currently defaults to 14).  This argument allows for special circumstances like a small popup for the Fore and Back color associated with the Pattern attribute control.

```pascal
PROCEDURE CreateColorPopup(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				widthInStdChar : LONGINT);
```

```python

def vs.CreateColorPopup(dialogID, itemID, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Examples
```pascal
PROCEDURE Example;

VAR

   dialog1 :INTEGER;

   result  :INTEGER;

PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

   CASE item OF

      SetupDialogC:

         BEGIN

            SetColorChoice(dialog1, 4, 1242);

         END;

      1:

         BEGIN

            GetColorChoice(dialog1, 4, result);

            AlrtDialog(Concat('color index: ', result));

         END;

   END;

END;

BEGIN

   dialog1 := CreateLayout('Example Dialog', FALSE, 'OK', 'Cancel');

   CreateColorPopup(dialog1, 4, 24);

   SetFirstLayoutItem(dialog1, 4);

   result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern

