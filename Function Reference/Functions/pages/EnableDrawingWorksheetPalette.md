# EnableDrawingWorksheetPalette

## Description
Enables/disables drawing for the specified worksheet or all displayed worksheet palettes if worksheet is nil.&lt;BR&gt;
&lt;BR&gt;
To improve speed and avoid flickering, it is highly recommended to disable drawing in worksheet palettes before performing several write operations in an opened worksheet. &lt;BR&gt;
Enable drawing back when the operations are completed. &lt;BR&gt;


```pascal
PROCEDURE EnableDrawingWorksheetPalette(
				enable    : BOOLEAN;
				worksheet : HANDLE);
```

```python

def vs.EnableDrawingWorksheetPalette(enable, worksheet):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|enable|BOOLEAN|Specifies if worksheet palettes' drawing  should be enabled or disabled.|
|worksheet|HANDLE|Handle to specific worksheet for which to enable/disable drawing;  Set it to nil to enable/disable drawing in all displayed worksheet palettes.|

## Examples
```pascal
{Disable drawing in all displayed worksheet palettes.}

EnableDrawingWorksheetPalette(false, nil);



{Write it worksheets ....}

...

...

...



{Enable back drawing in all displayed worksheet palettes.}

EnableDrawingWorksheetPalette(true, nil);
```

## Version
Availability: from Vectorworks 2009
## Category
* Worksheets

