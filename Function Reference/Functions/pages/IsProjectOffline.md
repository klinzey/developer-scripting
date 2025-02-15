# IsProjectOffline

## Description
Checks if current document is a Working File operating in Offline Mode.&lt;BR&gt;
&lt;BR&gt;
Offline Mode is when the Working File is opened and the Project File cannot be found.

```pascal
FUNCTION IsProjectOffline : BOOLEAN;
```

```python

def vs.IsProjectOffline():
    return BOOLEAN
```

## Returns
Returns True if current document is a Working File operating in Offline Mode.<BR>
Returns False on failure or not Project Sharing file, or not in Offline Mode.

## Version
Availability: from Vectorworks 2016
## Category
* Project Sharing

