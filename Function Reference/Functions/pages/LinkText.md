# LinkText

## Description
Creates a linked text field in a newly created symbol. The specified text is linked to a record field, whose value is displayed by the text object.&lt;BR&gt;
&lt;BR&gt;
LinkText must be called during symbol creation; the record to be associated with the linked text string must also exist at the time the link is created.

```pascal
PROCEDURE LinkText(
				h   : HANDLE;
				rec : DYNARRAY[] of CHAR;
				fld : DYNARRAY[] of CHAR);
```

```python

def vs.LinkText(h, rec, fld):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to text object that will be linked to record.|
|rec|DYNARRAY[] of CHAR|Name of record that will be linked to text string.|
|fld|DYNARRAY[] of CHAR|Name of field that will be linked to text string.|

## Examples
```pascal
BeginSym('Symbol #2');

  Oval(-3/4&quot;,1/2&quot;,3/4&quot;,-1/2&quot;);

  TextFont(3);

  TextSize(12.00037);

  TextJust(1);

  TextOrigin(0.8611111&quot;,0.5138889&quot;);

  BeginText;

   'Field 9 String'

  EndText;

  LinkText(LNewObj,'Sample Format','Field 1');

EndSym;

Record(LNewObj,'Sample Format');


```

## See Also
VS Functions:
[BeginSym](BeginSym.md)| [EndSym](EndSym.md)

## Version
Availability: from MiniCAD
## Category
* Database / Record

