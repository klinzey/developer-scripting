# GetFldType

## Description
Returns a constant indicating the data type of a specified field in the referenced record.

Please refer to the [[VS:Function Reference Appendix#Record - Worksheet Field Types |VectorScript Appendix]] for specific field data types and formatting.


For Plug-in Object Parameter Records, the field types are documented in the [[VS:Function Reference Appendix#Plug-in Object Parameter Record Field Types|VectorScript Appendix]].

```pascal
FUNCTION GetFldType(
				h : HANDLE;
				t : INTEGER): INTEGER;
```

```python
def vs.GetFldType(h, t):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to record.|
|t|INTEGER|Field index (range of 1 - n).|

## Remarks
Returns a constant indicating which type of field is specified by the field number &quot;t&quot; of record &quot;h&quot;.  The field type constants are listed in an appendix in the vectorscript manual.

In the appendix, the field types for worksheets and data records are listed, but the field types for parameter records (e.g., plug-in object records) are different...

[Data Record Field Types](../Appendix/pages/Appendix%20E%20-%20Miscellaneous%20Selectors.md#record---worksheet-field-types)

[PIO Records Field Types](../Appendix/pages/Appendix%20E%20-%20Miscellaneous%20Selectors.md#plug-in-object-parameter-record-field-types)


## Examples
==== VectorScript ====
```pascal
fieldType:=GetFldType(recordHandle,3);
```
==== Python ====
```python
fieldType = vs.GetFldType(recordHandle,3)
```

## Version
Availability: from All Versions

## Category
* Database @ Record

