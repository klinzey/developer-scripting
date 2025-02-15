# VerifyLayout

## Description
Checks a specified dialog layout for correct layout definition.

```pascal
FUNCTION VerifyLayout(dialogID : LONGINT) : BOOLEAN;
```

```python

def vs.VerifyLayout(dialogID):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout to be verified.|

## Returns
Returns FALSE if a problem was encountered defining the dialog, otherwise returns TRUE.

## Remarks
[DWD 1/20/00]

## Examples
```pascal
{verify the dialog layou is properly constructed}

	dialogOK := VerifyLayout(lEditID);



	IF (dialogOK &amp; rsAvailable) THEN

	BEGIN

		lmtestResult := RunLayoutDialog(lEditID,DriveSplashDialog);

	END;


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern

