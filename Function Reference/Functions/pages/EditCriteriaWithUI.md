# EditCriteriaWithUI

## Description
Edit a criteria string with Edit Criteria Dialog.

```pascal
FUNCTION EditCriteriaWithUI(VAR criteria : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.EditCriteriaWithUI(criteria):
    return (INTEGER, criteria)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|criteria|DYNARRAY[] of CHAR|Pass in a criteria to be edited, and output the modified criteria if the function result is TRUE.|

## Returns
The funtion returns the following values:<BR>
0 - failed. The input criteria is incorrect.<BR>
1 - The edit was OK<BR>
2 - The edit was Cancel<BR>


## Version
Availability: from Vectorworks 2014
## Category
* Utility

