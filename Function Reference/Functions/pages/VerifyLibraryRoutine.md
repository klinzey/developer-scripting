# VerifyLibraryRoutine

## Description
Verifies that a procedure or function call located in a VectorScript extension is registered and available for use in scripts.&lt;BR&gt;
&lt;BR&gt;
Call this function prior to using any call located in a VectorScript extension to ensure successful use of the call in a script.&lt;BR&gt;
&lt;BR&gt;
(A VectorScript extension is also known as an SDK Plug-in Library.  It is a plug-in that is developed using the Vectorworks SDK and the C++ language.  When installed in the Plug-ins folder it provides functions that may be called from VectorScript.  The VerifyLibraryRoutine function allows the script to determine if the function is available.)

```pascal
FUNCTION VerifyLibraryRoutine(routineName : STRING) : BOOLEAN;
```

```python

def vs.VerifyLibraryRoutine(routineName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|routineName|STRING|Name of function call to be verified.|

## Returns
Returns TRUE if the call is available, otherwise returns FALSE.

## Version
Availability: from VectorWorks9.0
## Category
* Utility

