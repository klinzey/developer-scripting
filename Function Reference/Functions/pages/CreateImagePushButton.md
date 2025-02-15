# CreateImagePushButton

## Description
Creates an image push button. Replaces CreateIconPushButton

```pascal
PROCEDURE CreateImagePushButton(
				dialogID       : LONGINT;
				controlID      : LONGINT;
				widthInStdChar : INTEGER;
				imageSpecifier : DYNARRAY[] of CHAR);
```

```python

def vs.CreateImagePushButton(dialogID, controlID, widthInStdChar, imageSpecifier):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The dialog identifier given by the command to create the dialog.|
|controlID|LONGINT|The identifier that should be assigned to the control.|
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|imageSpecifier|DYNARRAY[] of CHAR|The string identifier for the image. It should be of the form &quot;ResourceFileNameWithoutExtension/PathOfImageFile&quot;.|

## Version
Availability: from Vectorworks 2012
## Category
* Dialogs - Modern

