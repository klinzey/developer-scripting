# AlertInformDontShowAgain

## Description
Displays an alert dialog which provides the user with information about the result of a command with an option to not show the dialog again. It offers no user choices.&lt;BR&gt;
&lt;BR&gt;
The parameter 'arrOptions' is of type ARRAY [1..3] OF STRING;&lt;BR&gt;
arrOpt[1] - Saved setting category to save checkbox value&lt;BR&gt;
arrOpt[2] - Saved setting item to save checkbox value &lt;BR&gt;
arrOpt[3] - Specify the string to use in overriding the default 'Dont show this dialog again' checkbox string

```pascal
PROCEDURE AlertInformDontShowAgain(
				text       : DYNARRAY[] of CHAR;
				advice     : DYNARRAY[] of CHAR;
				minorAlert : BOOLEAN;
				arrOptions : ARRAY);
```

```python

def vs.AlertInformDontShowAgain(text, advice, minorAlert, arrOptions):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|text|DYNARRAY[] of CHAR|The information to be displayed.|
|advice|DYNARRAY[] of CHAR|The text to be added in a smaller font under the main information message.|
|minorAlert|BOOLEAN|The severity of the alert: minor(true) or major(false).|
|arrOptions|ARRAY|ARRAY [1..3] OF STRING; arrOpt[1] - Saved setting category to save checkbox value arrOpt[2] - Saved setting item to save checkbox value  arrOpt[3] - Specify a string to use in overriding the default 'Dont show this dialog again' checkbox string|

## Remarks
Created by TTF 1/9/2009

## Examples
```pascal
PROCEDURE Example;



VAR

	arrayText : ARRAY[1..3] OF STRING;



BEGIN

	arrayText[1] := 'DontShowDialogAgainCategory';

	arrayText[2] := 'DontShowDialogAgainItem'; {Should be unique for every AlertInformDontShowAgain}

	arrayText[3] := '';



	AlertInformDontShowAgain('This is an invalid item.', '', false, arrayText);

END;



RUN(Example);
```

## See Also
VS Functions:
[AlertInform](AlertInform.md)| [AlertQuestion](AlertQuestion.md)| [AlertCritical](AlertCritical.md)| [AlertQuestionDontShowAgain](AlertQuestionDontShowAgain.md)| [AlertCriticalHLink](AlertCriticalHLink.md)| [AlertInformHLink](AlertInformHLink.md)| [AlertInformHLinkN](AlertInformHLinkN.md)

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Predefined

