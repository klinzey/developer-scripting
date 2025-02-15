# SetItemToolTipText

## Description
Sets the tooltip text for list browsers, list boxes, edit controls, pull down menus, and enhanced static text.  Parameters nIndex and nSubIndex are used for list browsers and list boxes only.&lt;BR&gt;


```pascal
PROCEDURE SetItemToolTipText(
				nDialogID     : LONGINT;
				nComponentID  : LONGINT;
				strToolTip    : STRING;
				strSubToolTip : STRING;
				nIndex        : INTEGER;
				nSubIndex     : INTEGER);
```

```python

def vs.SetItemToolTipText(nDialogID, nComponentID, strToolTip, strSubToolTip, nIndex, nSubIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|nDialogID|LONGINT||
|nComponentID|LONGINT||
|strToolTip|STRING||
|strSubToolTip|STRING||
|nIndex|INTEGER||
|nSubIndex|INTEGER||

## Version
Availability: from VectorWorks 2008
## Category
* Dialogs - Modern

