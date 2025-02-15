# AddLBImage

## Description
Adds specified image resource to image list.&lt;BR&gt;
&lt;BR&gt;
Currently only one resource type is supported: the 'ics8' resource.  This is a 16x16 color icon.  Pass a value of 1 for the resourceType argument to indicate this type.  Call SetVSResourceFile to specify a resource file that contains the icons.

```pascal
FUNCTION AddLBImage(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				resourceType : INTEGER;
				resourceID   : INTEGER) : INTEGER;
```

```python

def vs.AddLBImage(dialogID, componentID, resourceType, resourceID):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|resourceType|INTEGER|type of image resource to be added|
|resourceID|INTEGER|the resource ID of image to add|

## See Also
VS Functions:
[SetVSResourceFile](SetVSResourceFile.md)| [CreateLB](CreateLB.md)| [InsertLBColumn](InsertLBColumn.md)| [SetLBControlType](SetLBControlType.md)| [SetLBItemDisplayType](SetLBItemDisplayType.md)| [InsertLBColumnDataItem](InsertLBColumnDataItem.md)| [SetLBItemUsingColumnDataItem](SetLBItemUsingColumnDataItem.md)| [InsertLBItem](InsertLBItem.md)| [EnableLBColumnLines](EnableLBColumnLines.md)

## Version
```diff
- AddLBImage is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser

