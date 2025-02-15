# GetCurrentMode

## Description
Returns the current application protection mode.&lt;BR&gt;
&lt;BR&gt;
Return values:&lt;BR&gt;
0 - Mode Not Set&lt;BR&gt;
1 - Full Mode&lt;BR&gt;
2 - Demo Mode&lt;BR&gt;
4 - Education Mode&lt;BR&gt;
8 - Student Mode&lt;BR&gt;
16 - Viewer Mode&lt;BR&gt;
32 - Unlicensed Mode&lt;BR&gt;
64 - Banner Mode&lt;BR&gt;
128 - Watermark New Files Mode&lt;BR&gt;
256 - Print Watermark Mode&lt;BR&gt;
512 - Save Educational File Format Mode&lt;BR&gt;
1024 - Open Educational File Format Mode&lt;BR&gt;
2048 - Vector Script Export Mode&lt;BR&gt;
4096 - Beta Serial Number Mode

```pascal
FUNCTION GetCurrentMode : INTEGER;
```

```python

def vs.GetCurrentMode():
    return INTEGER
```

## Examples
```pascal
Procedure TestMode;



Var

vwMode : LongInt;

ModeCheck : Boolean;





FUNCTION BitCheck(largeNum, smallNum :LONGINT) :BOOLEAN;

{Returns true if smallNum is a power of 2 present in largeNum.}



VAR

bit :INTEGER;

BEGIN

BitCheck := FALSE;

bit := 15;

while bit &gt; -1 do BEGIN

if largeNum &gt;= (2 ^ bit) then BEGIN

largeNum := largeNum - (2 ^ bit);

IF (2 ^ bit) = smallNum THEN BEGIN

BitCheck := TRUE;

bit := 0;

END;

END;

bit := bit - 1;

END;

END;



Begin

vwMode := GetCurrentMode;

{Educational or Student version}

ModeCheck := (BitCheck(vwMode, 4)) | (BitCheck(vwMode, 8));



AlrtDialog(Concat(vwMode,':',ModeCheck));

End;



Run (TestMode)


```

## Version
Availability: from VectorWorks10.0
## Category
* Utility

