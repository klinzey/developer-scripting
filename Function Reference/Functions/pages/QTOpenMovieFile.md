# QTOpenMovieFile

## Description
Creates or opens a QuickTime movie file for writing.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION QTOpenMovieFile(fileName : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.QTOpenMovieFile(fileName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Name of movie file.|

## Returns
An INTEGER index value identifying the open movie stream. A value of -1 indicates the stream could not be opened.

## Version
Availability: from VectorWorks8.5
## Category
* Special - QuickTime

