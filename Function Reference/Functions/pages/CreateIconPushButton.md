# CreateIconPushButton

## Description
Creates an icon push button with the specified icon ID and width in characters.

```pascal
PROCEDURE CreateIconPushButton(
				nDialogID      : LONGINT;
				nComponentID   : LONGINT;
				nIconID        : INTEGER;
				widthInStdChar : INTEGER);
```

```python

def vs.CreateIconPushButton(nDialogID, nComponentID, nIconID, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|nDialogID|LONGINT||
|nComponentID|LONGINT||
|nIconID|INTEGER|the index of the ICN# resource in the currently open rsrc file (or qtr on Windows)|
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Examples
```pascal
PROCEDURE Example;

VAR

   dialog1 :INTEGER;

   result  :INTEGER;

   boo     :BOOLEAN;

 

PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

END;

 

BEGIN

   boo := SetVSResourceFile('IP Resources');

   dialog1 := CreateLayout('Example Dialog', FALSE, 'OK', 'Cancel');

   CreateIconPushButton(dialog1, 4, 11021, 20);

   SetFirstLayoutItem(dialog1, 4);

   result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);
```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
```diff
- CreateIconPushButton is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.5
## Category
* Dialogs - Modern

