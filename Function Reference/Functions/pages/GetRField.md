# GetRField

## Description
Returns string description of a value in the specified record field.

```pascal
FUNCTION GetRField(
				h      : HANDLE;
				record : STRING;
				field  : STRING) : DYNARRAY[] of CHAR;
```

```python

def vs.GetRField(h, record, field):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|record|STRING|Name of record format.|
|field|STRING|Name of field to be queried.|

## Returns
Returns the field value as a variable length string.

## Remarks
Returns a string interpretation of the field from the specified record

## Examples
```pascal
PROCEDURE Example;



FUNCTION WriteFieldValues(h :HANDLE) :BOOLEAN;

VAR

   cnt     :INTEGER;

   recHand :HANDLE;

   recName :STRING;

   fldName :STRING;

BEGIN

   recName := GetName(GetRecord(h, NumRecords(h)));

   recHand := GetObject(recName);

   FOR cnt := 1 TO NumFields(recHand) DO BEGIN

      fldName := GetFldName(recHand, cnt);

      WriteLn(fldName, ': ', GetRField(h, recName, fldName));

   END;

END;



BEGIN

   ForEachObjectInLayer(WriteFieldValues, 2, 0, 4);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.5
## Category
* Database / Record

