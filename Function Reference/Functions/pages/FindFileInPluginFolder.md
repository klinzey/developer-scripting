# FindFileInPluginFolder

## Description
Searches for filename in all plug-in folders.  Returns TRUE if the file is found, FALSE otherwise.  If found, the result is returned in the path parameter.

```pascal
FUNCTION FindFileInPluginFolder(
				filename : DYNARRAY[] of CHAR;
				VAR path : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.FindFileInPluginFolder(filename):
    return (BOOLEAN, path)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filename|DYNARRAY[] of CHAR||
|path|DYNARRAY[] of CHAR||

## Examples
```pascal
PROCEDURE Example;

VAR

	filename, path :STRING;

BEGIN

	filename := 'Callout.vso';

	IF FindFileInPluginFolder(filename, path) 

		THEN AlrtDialog(path)

		ELSE AlrtDialog('Could not find file.');

END;

RUN(Example);


```

## Version
Availability: from VectorWorks12.0
## Category
* File I/O

