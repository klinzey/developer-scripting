# CreateTreeControl

## Description
Creates a Layout Manager tree control.

```pascal
PROCEDURE CreateTreeControl(
				nDialogID      : LONGINT;
				nComponentID   : LONGINT;
				widthInStdChar : INTEGER;
				heightInLines  : INTEGER);
```

```python

def vs.CreateTreeControl(nDialogID, nComponentID, widthInStdChar, heightInLines):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|nDialogID|LONGINT||
|nComponentID|LONGINT||
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|heightInLines|INTEGER||

## Examples
```pascal
PROCEDURE Example;

VAR

   dialog1 :INTEGER;

   result  :INTEGER;

   widthInStdChar, heightInLines :INTEGER;

   root1, root2, child1, child2 :INTEGER;



PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

   CASE item OF

      SetupDialogC:

         BEGIN

            root1 := InsertTreeControlItem(dialog1, 4, 'root1', -1, 0);

            child1 := InsertTreeControlItem(dialog1, 4, 'child1', root1, 0);

            child2 := InsertTreeControlItem(dialog1, 4, 'child2', root1, child1);

            root2 := InsertTreeControlItem(dialog1, 4, 'root2', -1, root1);

            child1 := InsertTreeControlItem(dialog1, 4, 'child1', root2, 0);

            child2 := InsertTreeControlItem(dialog1, 4, 'child2', root2, child1);

         END;

   END;

END;



BEGIN

   dialog1 := CreateLayout('Example Dialog', FALSE, 'OK', 'Cancel');

   widthInStdChar := 28;

   heightInLines := 8;

   CreateTreeControl(dialog1, 4, widthInStdChar, heightInLines);

   SetFirstLayoutItem(dialog1, 4);

   result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[GetTreeControlSelectedItem](GetTreeControlSelectedItem.md)| [InsertTreeControlItem](InsertTreeControlItem.md)| [RemoveTreeControlItem](RemoveTreeControlItem.md)| [GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks 2008
## Category
* Dialogs - Modern

