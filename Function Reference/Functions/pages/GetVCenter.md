# GetVCenter

## Description
Procedure GetVCenter returns the Vectorworks document coordinates at the center of the drawing window. 

```pascal
PROCEDURE GetVCenter(VAR center : REAL);
```

```python

def vs.GetVCenter():
    return center
```

## Parameters
|Name|Type|Description|
|---|---|---|
|center|REAL|Returns view center point.|

## Remarks
Returns the point which is in the center of the drawing window.<BR>
<BR>
[sd 8/18/98]

## Examples
```pascal
PROCEDURE GetWindowSizeProc;

CONST

	kLeftPaletteMargin    = 54;

	kRightPaletteMargin   = 176;

	kScrollMargin         = 18;

	kTopDocumentMargin    = 48;

	kRulerMargin          = 16;

	kBottomDocumentMargin = 50;

VAR

	ViewCenterX, ViewCenterY       :REAL;

	ViewWidth, ViewHeight          :REAL;

	ScnX1, ScnY1, ScnX2, ScnY2     :REAL;

	ViewX1, ViewY1, ViewX2, ViewY2 :REAL;

	LayerScale                     :REAL;

	TopBottomMargin                :REAL;

	LeftRightMargin                :REAL;

BEGIN

	LayerScale := GetLScale(ActLayer);

	GetVCenter(ViewCenterX, ViewCenterY);

	GetScreen(ScnX1, ScnY1, ScnX2, ScnY2);

	TopBottomMargin := kTopDocumentMargin + kBottomDocumentMargin;

	LeftRightMargin := 0;

	IF GetPref(22) THEN begin {Left Palette Margin Turned On}

		LeftRightMargin := LeftRightMargin + kLeftPaletteMargin;

	END;

	IF GetPref(23) THEN begin {Right Palette Margin Turned On}

		LeftRightMargin := LeftRightMargin + kRightPaletteMargin;

	END;

	IF GetPref(6) THEN BEGIN {Show Rulers}

		TopBottomMargin := TopBottomMargin + kRulerMargin;

		LeftRightMargin := LeftRightMargin + kRulerMargin;

	END;

	IF GetPref(7) THEN BEGIN {Show Scroll Bars}

		TopBottomMargin := TopBottomMargin + kScrollMargin;

		LeftRightMargin := LeftRightMargin + kScrollMargin;

	END;

	ViewWidth  := (ScnX2 - LeftRightMargin) * LayerScale / (72 * GetZoom / 100);

	ViewHeight := (ScnY2 - TopBottomMargin) * LayerScale / (72 * GetZoom / 100);

	ViewX1 := ViewCenterX - (ViewWidth  / 2) {+ (LeftRightMargin / 2)};

	ViewX2 := ViewCenterX + (ViewWidth  / 2) {- (LeftRightMargin / 2)};

	ViewY1 := ViewCenterY + (ViewHeight / 2) {- (TopBottomMargin / 2)};

	ViewY2 := ViewCenterY - (ViewHeight / 2) {+ (TopBottomMargin / 2)};

	Rect(ViewX1, ViewY1, ViewX2, ViewY2);

END;

RUN(GetWindowSizeProc);


```

## Version
Availability: from VectorWorks8.0
## Category
* View / Zoom

