# RunTempTool

## Description
Runs a temp tool. The call waits until the tool has finished. The callback function is notified for the tool events.

```pascal
PROCEDURE RunTempTool(
				toolCallback  : PROCEDURE;
				initialScroll : BOOLEAN);
```

```python

def vs.RunTempTool(toolCallback, initialScroll):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|toolCallback|PROCEDURE|Procedure that will be called with the tool events.
FUNCTION ToolCallback(action, msg1, msg2 : INTEGER) : INTEGER;|
|initialScroll|BOOLEAN|For experts. Pass FALSE if you want a simple temp tool. Setting it to TRUE will add one extra point (0,0) before the tool runs. This will make the tool scroll before the first click. This means that your tool handler must recognize and skip that extra fir|

## Examples
```pascal
PROCEDURE Test;

VAR

    pt1, pt2 : POINT;



    FUNCTION TempToolCallback(action, msg1, msg2 : LONGINT) : LONGINT;

    VAR pt : POINT;

    BEGIN

         TempToolCallback := 0;

         CASE action OF

             3: BEGIN {kOnToolDoSetupEventID}

		             vstSetHelpString ( 'Just click once.' );

             END;



             103 : BEGIN {kToolDrawEventID}

                 vstGetCurrPt2D( pt.x, pt.y );

                 vstDrawCoordLine( pt.x, pt.y, pt1.x, pt1.y );

                 vstDrawCoordLine( pt.x, pt.y, pt2.x, pt2.y );

             END;

         END;

    END;



BEGIN

    pt1.x := 0; pt1.y := 0;

    pt2.x := 100mm; pt2.y := 100mm;

    RunTempTool( TempToolCallback, FALSE );

END;

RUN( Test );
```

## Version
Availability: from Vectorworks 2010
## Category
* User Interactive

