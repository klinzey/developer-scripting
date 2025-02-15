# GetLastFileErr

## Description
Returns an error code indicating whether an error occured during a file operation.&lt;BR&gt;
&lt;BR&gt;
This function should be called after file I/O calls such as Open() or Rewrite().

```pascal
FUNCTION GetLastFileErr : INTEGER;
```

```python

def vs.GetLastFileErr():
    return INTEGER
```

## Examples
```pascal
UseDefaultFileErrorHandling(FALSE);

Open(Concat(pathName, fileName));

errorCode := GetLastFileErr;

IF errorCode &lt;&gt; 0 THEN

	CASE errorCode OF

		 2: AlrtDialog(Concat('The file &quot;', fileName, '&quot; cannot be processed because the hard drive is full.'));

		 4: AlrtDialog(Concat('End of file &quot;',   fileName, '&quot; reached prematurely.'));

		 5: AlrtDialog(Concat('The file &quot;', fileName, '&quot; is locked.'));

		 6: AlrtDialog(Concat('The file &quot;', fileName, '&quot; not found.'));

		10: AlrtDialog(Concat('The file &quot;', fileName, '&quot; currently in use by another program.'));

		13: AlrtDialog(Concat('The file path &quot;', pathName, '&quot; does not exist.'));

		OTHERWISE AlrtDialog(Concat('The file &quot;',fileName,'&quot; has encountered an undetermined error.'));

	END;


```

## Version
Availability: from VectorWorks8.5
## Category
* File I/O

