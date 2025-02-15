# SetColorChoice

## Description
Sets the choice for the color popup dialog control to the specified color index.  

```pascal
PROCEDURE SetColorChoice(
				dialogID   : LONGINT;
				itemID     : LONGINT;
				colorIndex : INTEGER);
```

```python

def vs.SetColorChoice(dialogID, itemID, colorIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|colorIndex|INTEGER||

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

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern

