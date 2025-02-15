# AlertSetAlwaysDoVal

## Description
Set the 'always do' value for the AlertQuestionDontShowAgain and AlertInformDontShowAgain standard dialogs.

```pascal
PROCEDURE AlertSetAlwaysDoVal(
				category : DYNARRAY[] of CHAR;
				item     : DYNARRAY[] of CHAR;
				value    : INTEGER);
```

```python

def vs.AlertSetAlwaysDoVal(category, item, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|category|DYNARRAY[] of CHAR|category name of the value.|
|item|DYNARRAY[] of CHAR|item name in the category.|
|value|INTEGER|new value for the default. Pass in -1 for the entry to be cleared out and the dialog to show up again.|

## See Also
VS Functions:
[AlertQuestionDontShowAgain](AlertQuestionDontShowAgain.md)| [AlertInformDontShowAgain](AlertInformDontShowAgain.md)

## Version
Availability: from Vectorworks 2012
## Category
* Dialogs - Predefined

