# SetStaticTextStyle

## Description
Sets the style for the Layout Manager static Text&lt;BR&gt;
&lt;BR&gt;
Plain 0&lt;BR&gt;
Bold 1&lt;BR&gt;
Italic 2&lt;BR&gt;
Underline 4&lt;BR&gt;
&lt;BR&gt;
Can combine styles (bold + italic = 3)

```pascal
PROCEDURE SetStaticTextStyle(
				dialogID    : LONGINT;
				componentID : LONGINT;
				style       : INTEGER);
```

```python

def vs.SetStaticTextStyle(dialogID, componentID, style):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|componentID|LONGINT||
|style|INTEGER||

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Modern

