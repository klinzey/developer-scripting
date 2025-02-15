# AlertQuestionDontShowAgain

## Description
Displays an alert dialog which alerts the user to a condition or situation that requires the user's decision and input before preceding; such as an impending action with potentially destructive or irreversible consequences with the option to always do the selected action and not show the dialog again. The message should be in the form of a question.&lt;BR&gt;
&lt;BR&gt;
The parameter 'arrOptions' is of type ARRAY [1..3] OF STRING;&lt;BR&gt;
arrOpt[1] - Saved setting category to save checkbox value&lt;BR&gt;
arrOpt[2] - Saved setting item to save checkbox value &lt;BR&gt;
arrOpt[3] - Specify a string to use in overriding the default 'Always do the selection action' checkbox string

```pascal
FUNCTION AlertQuestionDontShowAgain(
				question           : DYNARRAY[] of CHAR;
				advice             : DYNARRAY[] of CHAR;
				defaultButton      : INTEGER;
				OKOverrideText     : DYNARRAY[] of CHAR;
				CancelOverrideText : DYNARRAY[] of CHAR;
				customButtonAText  : DYNARRAY[] of CHAR;
				customButtonBText  : DYNARRAY[] of CHAR;
				arrOptions         : ARRAY) : INTEGER;
```

```python

def vs.AlertQuestionDontShowAgain(question, advice, defaultButton, OKOverrideText, CancelOverrideText, customButtonAText, customButtonBText, arrOptions):
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
|arrOptions|ARRAY|ARRAY [1..3] OF STRING;    arrOpt[1] - Saved setting category to save checkbox value    arrOpt[2] - Saved setting item to save checkbox value     arrOpt[3] - Specify a string to use in overriding the default 'Always do the selection action' checkbox string|

## Returns
Return Values<BR>
0:  the negative button was hit<BR>
1:  the positive button was hit<BR>
2:  custom button A was hit<BR>
3:  custom button B was hit

## Remarks
Created by TTF 1/9/2009

## Examples
```pascal
PROCEDURE Example;



VAR

	result :INTEGER;

	arrayText : ARRAY[1..3] OF STRING;



BEGIN

	arrayText[1] := 'DontShowDialogAgainCategory';

	arrayText[2] := 'DontShowDialogAgainItem'; {Should be unique for every AlertQuestionDontShowAgain}

	arrayText[3] := '';



	result := AlertQuestionDontShowAgain('Do you want to continue?', '', 0, 'Yes', 'No', '', '', arrayText);

END;



RUN(Example);
```

## See Also
VS Functions:
[AlertInform](AlertInform.md)| [AlertQuestion](AlertQuestion.md)| [AlertCritical](AlertCritical.md)| [AlertInformDontShowAgain](AlertInformDontShowAgain.md)| [AlertCriticalHLink](AlertCriticalHLink.md)| [AlertInformHLink](AlertInformHLink.md)| [AlertInformHLinkN](AlertInformHLinkN.md)

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Predefined

