# CopySymbol

## Description
Procedure CopySymbol will copy a symbol into the active document from a user specified source document. &lt;BR&gt;
&lt;BR&gt;
If the filename includes a fully qualified path, the path has to use the appropriate notation for the local operating system:&lt;br&gt; 
&lt;dir&gt;Macintosh HD:Applications:Vectorworks:Plug-Ins:Data:Notes.txt&lt;/dir&gt;
&lt;dir&gt;C:\Program Files\Vectorworks\Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename includes a path relative to the location of the Vectorworks executable, the subfolder delimiters have to be backslashes:&lt;br&gt;
&lt;dir&gt;Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename does not include a path, the file is assumed to exist in the same folder as the Vectorworks executable.

```pascal
FUNCTION CopySymbol(
				filePath : STRING;
				symbol   : STRING) : BOOLEAN;
```

```python

def vs.CopySymbol(filePath, symbol):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filePath|STRING|File path to document, relative to the application folder.|
|symbol|STRING|Name of symbol to import.|

## Returns
Returns a BOOLEAN value indicating the success or failure of the import operation.

## Examples
```pascal
PROCEDURE CopySym;

VAR

	theSymbolName :STRING;

BEGIN

	theSymbolName := 'Fax';

	IF CopySymbol('Object Libraries\Office Equipment.mcd', theSymbolName) 

		THEN Symbol(theSymbolName, 0, 0, 0);

END;

RUN(CopySym);
```

## Version
Availability: from MiniCAD
## Category
* Objects - Symbols

