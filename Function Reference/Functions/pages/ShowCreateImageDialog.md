# ShowCreateImageDialog

## Description
Displays a dialog that allows the user to select an image file from which a new image resource is created.

```pascal
FUNCTION ShowCreateImageDialog : HANDLE;
```

```python

def vs.ShowCreateImageDialog():
    return HANDLE
```

## Returns
Returns the handle to the newly created image resource if successful; nil otherwise.

## Examples
```pascal
imageHandle := ShowCreateImageDialog;
```

## Version
Availability: from VectorWorks10.0
## Category
* Document Attributes

