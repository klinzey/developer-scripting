# IsLWByClass

## Description
Function IsLWByClass returns whether a class line weight is used for the referenced object.

```pascal
FUNCTION IsLWByClass(h : HANDLE) : BOOLEAN;
```

```python

def vs.IsLWByClass(h):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Remarks
Returns an indication of whether the class line weight is used for the object referenced by h.<BR>
[sd 8/19/98]

## Examples
```pascal
PROCEDURE Example;

VAR

   symDefHandle, h :HANDLE;



PROCEDURE AlertMe;

BEGIN

   Message(GetSDName(symDefHandle));

   SetSelect(h);

END;



BEGIN

   DSelectAll;

   ClrMessage;

   symDefHandle := FSymDef;

   WHILE symDefHandle &lt;&gt; NIL DO BEGIN

      h := FInSymDef(symDefHandle);

      WHILE h &lt;&gt; NIL DO BEGIN

         IF IsLWByClass(h) THEN AlertMe;

         h := NextObj(h);

      END;

      symDefHandle := NextObj(symDefHandle);

   END;

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.0
## Category
* Object Attributes

