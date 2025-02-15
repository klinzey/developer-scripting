# AlertCritical

## Description
Informs the user of a serious problem that requires intervention or correction before work can continue.

```pascal
PROCEDURE AlertCritical(
				text   : DYNARRAY[] of CHAR;
				advice : DYNARRAY[] of CHAR);
```

```python

def vs.AlertCritical(text, advice):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|text|DYNARRAY[] of CHAR|The information to be displayed.|
|advice|DYNARRAY[] of CHAR|The text to be added in a smaller font under the main information message.|

## Remarks
Created by TTF 1/18/2005

## Examples
```pascal
AlertCritical('Out of Memory', '');
```

## See Also
VS Functions:
[AlertInform](AlertInform.md)| [AlertQuestion](AlertQuestion.md)| [AlertInformDontShowAgain](AlertInformDontShowAgain.md)| [AlertQuestionDontShowAgain](AlertQuestionDontShowAgain.md)| [AlertCriticalHLink](AlertCriticalHLink.md)| [AlertInformHLink](AlertInformHLink.md)| [AlertInformHLinkN](AlertInformHLinkN.md)

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Predefined

