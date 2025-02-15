# AlertInform

## Description
Displays an alert dialog which provides the user with information about the result of a command. It offers no user choices.

```pascal
PROCEDURE AlertInform(
				text       : DYNARRAY[] of CHAR;
				advice     : DYNARRAY[] of CHAR;
				minorAlert : BOOLEAN);
```

```python

def vs.AlertInform(text, advice, minorAlert):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|text|DYNARRAY[] of CHAR|The information to be displayed.|
|advice|DYNARRAY[] of CHAR|The text to be added in a smaller font under the main information message.|
|minorAlert|BOOLEAN|The severity of the alert: minor(true) or major(false).|

## Remarks
Created by TTF 1/18/2005

## Examples
```pascal
AlertInform('That item is not a valid item', '',isMinorAlert);
```

## See Also
VS Functions:
[AlertQuestion](AlertQuestion.md)| [AlertCritical](AlertCritical.md)| [AlertInformDontShowAgain](AlertInformDontShowAgain.md)| [AlertQuestionDontShowAgain](AlertQuestionDontShowAgain.md)| [AlertCriticalHLink](AlertCriticalHLink.md)| [AlertInformHLink](AlertInformHLink.md)| [AlertInformHLinkN](AlertInformHLinkN.md)

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Predefined

