# AlertQuestion

## Description
Displays an alert dialog which alerts the user to a condition or situation that requires the user's decision and input before preceding; such as an impending action with potentially destructive or irreversible consequences. The message should be in the form of a question.			&lt;BR&gt;


```pascal
FUNCTION AlertQuestion(
				question           : DYNARRAY[] of CHAR;
				advice             : DYNARRAY[] of CHAR;
				defaultButton      : INTEGER;
				OKOverrideText     : DYNARRAY[] of CHAR;
				CancelOverrideText : DYNARRAY[] of CHAR;
				customButtonAText  : DYNARRAY[] of CHAR;
				customButtonBText  : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.AlertQuestion(question, advice, defaultButton, OKOverrideText, CancelOverrideText, customButtonAText, customButtonBText):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|question|DYNARRAY[] of CHAR|The question to display|
|advice|DYNARRAY[] of CHAR|The text to be added in a smaller font under the main information/message|
|defaultButton|INTEGER|Specifies which button is to be made the default
0:	the negative button is the default
1:	the positive button is the default
2:	custom button A is the default 
3:	custom button B is the default |
|OKOverrideText|DYNARRAY[] of CHAR|Specifies a string to use in overriding the 'OK' string|
|CancelOverrideText|DYNARRAY[] of CHAR|Specifies a string to use in overriding the 'Cancel' string|
|customButtonAText|DYNARRAY[] of CHAR|Specifies a string to use for an optional custom button A|
|customButtonBText|DYNARRAY[] of CHAR|Specifies a string to use for a second optional custom button B|

## Returns
Return Values<BR>
0:  the negative button was hit<BR>
1:  the positive button was hit<BR>
2:  custom button A was hit<BR>
3:  custom button B was hit

## Remarks
Created by TTF 1/18/2005

## Examples
```pascal
PROCEDURE Example;

BEGIN

  AlrtDialog('AlrtDialog');

  AlertInform('AlertInform', 'advice', FALSE);

  AlertCritical('AlertCritical', 'advice');

  Message(YNDialog('YNDialog'));

  Message(AlertQuestion('question', 'advice', 1, 'ok', 'cancel', 'a', 'b'));

END;

RUN(Example);
```

## See Also
VS Functions:
[AlertInform](AlertInform.md)| [AlertCritical](AlertCritical.md)| [AlertInformDontShowAgain](AlertInformDontShowAgain.md)| [AlertQuestionDontShowAgain](AlertQuestionDontShowAgain.md)| [AlertCriticalHLink](AlertCriticalHLink.md)| [AlertInformHLink](AlertInformHLink.md)| [AlertInformHLinkN](AlertInformHLinkN.md)

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Predefined

