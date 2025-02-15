# New Functions 

[[VS:Vectorworks 2010 New Functions]]


# List of deprecated functions

## Dialogs - Classic

* __AddButton__
* __AddChoiceItem__
* __AddField__
* __AddGroupBox__
* __AddHelpItem__
* __BeginDialog__
* __ClrDialog__
* __DialogEvent__
* __DrawDialog__
* __EndDialog__
* __GetDialog__
* __SetTitle__

## Dialogs - Handler

* __DelChoice__
* __GetChoiceStr__
* __GetField__
* __GetSelChoice__
* __InsertChoice__
* __ItemSel__
* __NumChoices__
* __SelChoice__
* __SelField__
* __SetField__
* __SetHelpString__
* __SetItem__
* __SetItemEnable__
* __SetTextEditable__

## Textures

* __GetTexMapBool__
* __GetTexMapInt__
* __GetTexMapReal__
* __GetTextureRef__
* __SetDefaultTexMap__
* __SetTexMapBool__
* __SetTexMapInt__
* __SetTexMapReal__
* __SetTextureRef__

# Layout Manager API Match Table

## Dialogs - Classic

| Legacy APIs | Layout Manager APIs |
|-------------|---------------------|
| __AddButton__ | [CreatePushButton](../../Function%20Reference/Functions/pages/CreatePushButton.md)<br>[CreateCheckBox](../../Function%20Reference/Functions/pages/CreateCheckBox.md)<br>[CreateRadioButton](../../Function%20Reference/Functions/pages/CreateRadioButton.md) |
| __AddChoiceItem__ | [CreatePullDownMenu](../../Function%20Reference/Functions/pages/CreatePullDownMenu.md) |
| __AddField__ | [CreateStaticText](../../Function%20Reference/Functions/pages/CreateStaticText.md)<br>[CreateEditText](../../Function%20Reference/Functions/pages/CreateEditText.md)<br>[CreateEditTextBox](../../Function%20Reference/Functions/pages/CreateEditTextBox.md)<br>[CreateEditInteger](../../Function%20Reference/Functions/pages/CreateEditInteger.md)<br>[CreateEditReal](../../Function%20Reference/Functions/pages/CreateEditReal.md) |
| __AddGroupBox__ | [CreateGroupBox](../../Function%20Reference/Functions/pages/CreateGroupBox.md)<br>[CreateCheckBoxGroupBox](../../Function%20Reference/Functions/pages/CreateCheckBoxGroupBox.md)<br>[CreateRadioButtonGroupBox](../../Function%20Reference/Functions/pages/CreateRadioButtonGroupBox.md) |
| __AddHelpItem__ | [SetHelpText](../../Function%20Reference/Functions/pages/SetHelpText.md) |
| __BeginDialog__ | - |
| __ClrDialog__ | - |
| __DialogEvent__ | - |
| __DrawDialog__ | - |
| __EndDialog__ | - |
| __GetDialog__ | - |
| __SetTitle__ | - |

## Dialogs - Handler

| Legacy APIs | Layout Manager APIs |
|-------------|---------------------|
| __DelChoice__ | [RemoveChoice](../../Function%20Reference/Functions/pages/RemoveChoice.md) |
| __GetChoiceStr__ | [GetChoiceText](../../Function%20Reference/Functions/pages/GetChoiceText.md) |
| __GetField__ | [GetItemText](../../Function%20Reference/Functions/pages/GetItemText.md)<br>[GetMultilineText](../../Function%20Reference/Functions/pages/GetMultilineText.md) |
| __GetSelChoice__ | [GetSelectedChoiceInfo](../../Function%20Reference/Functions/pages/GetSelectedChoiceInfo.md) |
| __InsertChoice__ | [AddChoice](../../Function%20Reference/Functions/pages/AddChoice.md) |
| __ItemSel__ | [GetBooleanItem](../../Function%20Reference/Functions/pages/GetBooleanItem.md) |
| __NumChoices__ | [GetChoiceCount](../../Function%20Reference/Functions/pages/GetChoiceCount.md) |
| __SelChoice__ | [SelectChoice](../../Function%20Reference/Functions/pages/SelectChoice.md) |
| __SelField__ | [SelectEditText](../../Function%20Reference/Functions/pages/SelectEditText.md) |
| __SetField__ | [SetItemText](../../Function%20Reference/Functions/pages/SetItemText.md) |
| __SetItem__ | [SetBooleanItem](../../Function%20Reference/Functions/pages/SetBooleanItem.md) |
| __SetHelpString__ | [SetHelpText](../../Function%20Reference/Functions/pages/SetHelpText.md) |
| __SetItemEnable__ | [EnableItem](../../Function%20Reference/Functions/pages/EnableItem.md) |
| __SetTextEditable__ | [EnableTextEdit](../../Function%20Reference/Functions/pages/EnableTextEdit.md) |

## Textures

| Legacy APIs | Layout Manager APIs |
|-------------|---------------------|
| __GetTexMapBool__ | [GetTexMapBoolN](../../Function%20Reference/Functions/pages/GetTexMapBoolN.md) |
| __GetTexMapInt__ | [GetTexMapIntN](../../Function%20Reference/Functions/pages/GetTexMapIntN.md) |
| __GetTexMapReal__ | [GetTexMapRealN](../../Function%20Reference/Functions/pages/GetTexMapRealN.md) |
| __GetTextureRef__ | [GetTextureRefN](../../Function%20Reference/Functions/pages/GetTextureRefN.md) |
| __SetDefaultTexMap__ | [SetDefaultTexMapN](../../Function%20Reference/Functions/pages/SetDefaultTexMapN.md) |
| __SetTexMapBool__ | [SetTexMapBoolN](../../Function%20Reference/Functions/pages/SetTexMapBoolN.md) |
| __SetTexMapInt__ | [SetTexMapIntN](../../Function%20Reference/Functions/pages/SetTexMapIntN.md) |
| __SetTexMapReal__ | [SetTexMapRealN](../../Function%20Reference/Functions/pages/SetTexMapRealN.md) |
| __SetTextureRef__ | [SetTextureRefN](../../Function%20Reference/Functions/pages/SetTextureRefN.md) |

