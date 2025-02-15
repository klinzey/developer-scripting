# Appendix G - Object Selectors

## Dimensions

| Object Setting | Selector | Setting Value | Function Type |
|----------------|----------|---------------|---------------|
| Dimension Standard | 0 | 1 (Arch) | [VS:GetObjectVariableInt] |
| | | 2 (ASME) | " |
| | | 3 (BSI) | " |
| | | 4 (DIN) | " |
| | | 5 (ISO) | " |
| | | 6 (JIS) | " |
| | | 7 (SIA) | " |
| | | 8 (ASME Dual Side-by-Side) | " |
| | | 9 (ASME Dual Stacked) | " |
| Arrows Inside | 3 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Text Box (Primary Value) | 5 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Primary Dimension Text | 6 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Display Starting Witness Line | 7 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Display Ending Witness Line | 8 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Leader Text (Primary) | 9 | 31 character STRING value | [VS:GetObjectVariableString] |
| Trailer Text (Primary) | 10 | 31 character STRING value | [VS:GetObjectVariableString] |
| Dimension Tolerancing | 11 | 0 (no tolerance) | [VS:GetObjectVariableInt] |
| | | 1 (single tolerance) | " |
| | | 2 (double tolerance) | " |
| | | 3 (limit tolerance) | " |
| Dimension Text Offset | 15 | REAL | [VS:GetObjectVariableReal] |
| Dimension Text Font Size | 17 | REAL | [VS:GetObjectVariableReal] |
| Dimension Text Font Style | 19 | 0 (Plain) | [VS:GetObjectVariableInt] |
| | | 1 (Bold) | " |
| | | 2 (Italic) | " |
| | | 4 (Underline) | " |
| | | 8 (Outline [Mac only]) | " |
| | | 16 (Shadow [Mac only]) | " |
| Dimension Precision (Primary) | 20 | For decimal precision: value is digits after decimal point. | [VS:GetObjectVariableLongInt] |
| | | For fractional precision: value is power of 2 for fractional denominator (1 for 1/2, 2 for 1/4, 3 for 1/8, 4 for 1/16, etc). | " |
| | | For angular precision: 1 for whole number, 2 (degrees min), 3 (degrees min sec), 5 (x.x angular units), 6 (x.xx), 7 (x.xxx), 8 (x.xxxx), 9 (x.xxxxx), 10 (x.xxxxxx), 11 (x.xxxxxxx), 12 (x.xxxxxxxx) | " |
| Dimension Precision (Secondary) | 21 | For decimal precision: value is digits after decimal point. | [VS:GetObjectVariableLongInt] |
| | | For fractional precision: value is power of 2 for fractional denominator (1 for 1/2, 2 for 1/4, 3 for 1/8, 4 for 1/16, etc). | " |
| | | For angular precision: value is not used. | " |
| Use Text Box (Secondary) | 22 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Secondary Dimension Text | 23 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Leader Text (Secondary) | 24 | 31 character STRING value | [VS:GetObjectVariableString] |
| Trailer Text (Secondary) | 25 | 31 character STRING value | [VS:GetObjectVariableString] |
| Dimension Type | 26 | 0 (Constrained) | [VS:GetObjectVariableInt] |
| | | 1 (Unconstrained) | " |
| | | 2 (Ordinate) | " |
| | | 3 (Radial) | " |
| | | 4 (Diameter) | " |
| | | 5 (Angular) | " |
| Dimension Standard Name | 27 | STRING value | [VS:GetObjectVariableString] |
| Dimension Font ID | 28 | Font ID | [VS:GetObjectVariableInt] |
| Calculate Dim Text Position | 29 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Force Dim Text Inside | 30 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Angle is Reference | 31 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Only Primary | 32 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Only Secondary | 33 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Top Tolerance Value | 34 | REAL value | [VS:GetObjectVariableReal] |
| Bottom Tolerance Value | 35 | REAL value | [VS:GetObjectVariableReal] |
| Top Tolerance String | 36 | STRING | [VS:GetObjectVariableString] |
| Bottom Tolerance String | 37 | STRING | [VS:GetObjectVariableString] |
| Use Tolerance Strings | 38 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Flip Text | 39 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Dimension Text Font Size | 40 | in points | [VS:GetObjectVariableReal] |
| Dimension Text Rotation | 41 | 0 = Aligned, 1 = Horizontal, 2 = Horiz/Vertical | [VS:GetObjectVariableInt] |
| Dim Text Offset Above Line | 43 | REAL (current units) | [VS:GetObjectVariableReal] |
| Dim Text Offset | 44 | REAL value | [VS:GetObjectVariableReal] |
| Dimension Offset | 45 | REAL (current units) | [VS:GetObjectVariableReal] |
| Show Elevation Dimension (SIA Only) | 46 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Elevation Dimension Value (SIA Only) | 47 | REAL value | [VS:GetObjectVariableReal] |
| Leader Text for Elevation Dimension (SIA Only) | 48 | 31 character STRING value | [VS:GetObjectVariableString] |
| Trailer Text for Elevation Dimension (SIA Only) | 49 | 31 character STRING value | [VS:GetObjectVariableString] |
| Leader Arrow Width | 50 | INTEGER value | [VS:GetObjectVariableInt] |
| Text Style | 51 | Text Style Index | [VS:GetObjectVariableLongInt] |
| Text Position | 52 | LONGINT value | [VS:GetObjectVariableLongInt] |
| Witness Override Settings | 1235 | 0 = Standard | [VS:GetObjectVariableInt] |
| | | 1 = Single Custom Length | |
| | | 2 = Multiple Custom Length | |
| | | 3 = Single Custom Offset | |
| | | 4 = Multiple Custom Offset | |
| Witness Line Length for Single Custom or Starting Multiple Custom | 1236 | REAL value | [VS:GetObjectVariableReal] |
| Witness Line Length for Ending Witness Line | 1237 | REAL value | [VS:GetObjectVariableReal] |
| Witness Line offset for Single Custom or Starting Multiple Custom | 1238 | REAL value | [VS:GetObjectVariableReal] |
| Witness Line offset for Ending Witness Line | 1239 | REAL value | [VS:GetObjectVariableReal] |
| Leader Line Visibility | 1240 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Leader Line Marker Type | 1241 | Marker Type | [VS:GetObjectVariableLongInt] |
| Leader Line Marker Size | 1242 | INTEGER | [VS:GetObjectVariableInt] |
| Leader Line Marker Angle | 1243 | INTEGER | [VS:GetObjectVariableInt] |
| Leader Line Marker Thickness Basis | 1244 | INTEGER | [VS:GetObjectVariableInt] |
| Leader Line Marker Thickness | 1245 | INTEGER | [VS:GetObjectVariableInt] |
| Leader Line Marker Visibility | 1246 | -1 = Undefined Visibility | [VS:GetObjectVariableInt] |
| | | 0 = Invisible | |
| | | 1 = Visible | |
| The width of the marker for the leader line | 1247 | INTEGER | [VS:GetObjectVariableInt] |
| Dimension Text Style | 1248 | LONGINT | [VS:GetObjectVariableLongInt] |
| Use SIA Custom Elevation Dimension | 1249 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Compact mode for Radial Dimensions | 1250 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Witness Line Perp to Chord | 1250 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |
| Arc Indicator | 1251 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |
| Clockwise Arc | 1252 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |
| Dim Note Text | 1233 | The note text under dimension line or value. | [VS:GetObjectVariableString] |
| Viewport RePosition Dimension Text | 1042 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Is Design Layer Section Viewport | 1043 | TRUE or FALSE (read only) | [VS:GetObjectVariableBoolean] |
| Display Flattened Viewport in Wireframe (OBSOLETE) | 1044 | TRUE or FALSE (read only) | [VS:GetObjectVariableBoolean] |
| The viewport page symbol scale | 1045 | REAL | [VS:GetObjectVariableReal] |
| Viewport Detail Level low detail = 0, medium detail = 1, high detail = 2 | 1047 | INTEGER | [VS:GetObjectVariableInt] |
| Viewport Is Horizontal Section | 1048 | Read Only | [VS:GetObjectVariableBoolean] |
| Viewport Is Section Viewport | 1054 | Read Only | [VS:GetObjectVariableBoolean] |

## Lights

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Light On | 50 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Brightness | 51 | REAL (percentage) | [VS:GetObjectVariableReal] |
| Shadow Casting On | 53 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Light Type | 55 | 1 (Directional) | [VS:GetObjectVariableInt] |
| | | 2 (Point) | " |
| | | 3 (Spotlight) | " |
| Light Pan Angle | 57 | REAL value | [VS:GetObjectVariableReal] |
| Light Tilt Angle | 58 | REAL value | [VS:GetObjectVariableReal] |
| Distance Falloff Type | 59 | 0 (None) | [VS:GetObjectVariableInt] |
| | | 1 (Smooth) | " |
| | | 2 (Sharp) | " |
| Angular Falloff Type | 60 | 0 (none) | [VS:GetObjectVariableInt] |
| | | 1 (Normal) | " |
| | | 2 (Smooth) | " |
| | | 3 (Sharp) | " |
| Light Spread Angle | 61 | REAL value | [VS:GetObjectVariableReal] |
| Beam Angle | 62 | REAL value | [VS:GetObjectVariableReal] |
| Light Lit Fog | 63 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Soft Shadows | 64 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Emitter | 1620 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Emitter Brightness | 1621 | REAL | [VS:GetObjectVariableReal] |
| Emitter Brightness Units | 1622 | INTEGER | [VS:GetObjectVariableInt] |
| | | 0 (Lumens) | |
| | | 1 (Candelas) | |
| | | 2 (Lux) | |
| | | 3 (Footcandles) | |
| Use Color Temperature | 1623 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Color Temperature | 1624 | REAL | [VS:GetObjectVariableReal] |
| Caustic Photons | 1625 | REAL | [VS:GetObjectVariableReal] |
| | | 0 (None) | |
| | | 1000 (Low) | |
| | | 100000 (Medium) | |
| | | 1000000 (High) | |
| | | 10000000 (Very High) | |
| Use Caustics Only | 64 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |

## Symbols

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Symbol Light Multiplier | 100 | REAL value | [VS:GetObjectVariableReal] |
| Symbol Scale Type | 101 | 1 (None) | [VS:GetObjectVariableInt] |
| | | 1 (None) | " |
| | | 2 (Symmetric) | " |
| | | 3 (Asymmetric) | " |
| Symbol X Scale Factor | 102 | REAL value | [VS:GetObjectVariableReal] |
| Symbol Y Scale Factor | 103 | REAL value | [VS:GetObjectVariableReal] |
| Symbol Z Scale Factor | 104 | REAL value | [VS:GetObjectVariableReal] |
| Symbol Insert Mode | 125 | 0 (On center of wall) | [VS:GetObjectVariableInt] |
| | | 1 (On edge of wall) | " |
| Symbol Break Mode | 126 | 1 (Full break) | [VS:GetObjectVariableInt] |
| | | 2 (Full break no caps) | " |
| | | 3 (Half break) | " |
| | | 4 (no break) | " |
| Insert As Group | 127 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Class of Symbol Definition | 128 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Symbol Definition Insert Into Walls | 129 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Symbol Definition Page Based | 130 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Whether the symbol's height will be bound by story levels | 131 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |

## Roofs, Floors, Columns

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Slab Type | 172 | 1 (Roof) | [VS:GetObjectVariableInt] |
| | | 2 (Floor) | " |
| | | 3 (Column) | " |
| Slab Thickness | 173 | REAL (current units) | [VS:GetObjectVariableReal] |
| Slab Height | 174 | REAL (current units) (1) | [VS:GetObjectVariableReal] |
| Roof Edge Miter Type | 180 | 1 (Vertical) | [VS:GetObjectVariableInt] |
| | | 2 (Horizontal) | " |
| | | 3 (Compound) | " |
| Double Miter Ratio Value | 181 | REAL value (3) | [VS:GetObjectVariableReal] |
| Roof Rise | 182 | REAL (current units) (2) | [VS:GetObjectVariableReal] |
| Roof Run | 183 | REAL (current units) (2) | [VS:GetObjectVariableReal] |

**Notes:**
1. Height is the bottom of the slab for floors and columns, elevation of the roof axis for roofs.
2. Roof only.
3. A value between 0 and 1 indicating the percentage of the miter which is vertical.

## Layer

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Layer Ambient Status | 150 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Layer Ambient Brightness | 151 | REAL value | [VS:GetObjectVariableReal] |
| Layer Visibility | 153 | -1 (Invisible) | [VS:GetObjectVariableInt] |
| | | 0 (Normal) | " |
| | | 2 (Grayed) | " |
| Layer Type | 154 | INTEGER | [VS:GetObjectVariableInt] |
| Layer Printing DPI | 155 | INTEGER | [VS:GetObjectVariableInt] |
| Layer Renderworks Background | 591 | LONGINT | [VS:GetObjectVariableLongInt] |
| Layer Repaginate | 156 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Layer Height | 157 | REAL (current units) | [VS:GetObjectVariableReal] |
| Layer Thickness | 158 | REAL (current units) | [VS:GetObjectVariableReal] |
| Sheet Layer Title | 159 | STRING value | [VS:GetObjectVariableString] |
| HDRI Layer | 592 | LONGINT | [VS:GetObjectVariableLongInt] |

## Layer Link

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Source Layer Name | 160 | STRING value | [VS:GetObjectVariableString] |
| Project 2D Objects | 161 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Layer Expanded Sheet Name | 162 | STRING value | [VS:GetObjectVariableString] |

## Viewports

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Projection Type | 1000 | INTEGER | [VS:GetObjectVariableInt] |
| Render Type | 1001 | INTEGER | [VS:GetObjectVariableInt] |
| Perspective Distance | 1002 | REAL | [VS:GetObjectVariableReal] |
| Scale | 1003 | REAL | [VS:GetObjectVariableReal] |
| Needs Update | 1004 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Project 2D | 1005 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Render Background | 1006 | LONGINT | [VS:GetObjectVariableLongInt] |
| View Type | 1007 | INTEGER | [VS:GetObjectVariableInt] |
| Line Weight Scale | 1008 | REAL | [VS:GetObjectVariableReal] |
| Arrowhead Scale | 1009 | REAL | [VS:GetObjectVariableReal] |
| Dashed Line Scale | 1010 | REAL | [VS:GetObjectVariableReal] |
| Hatch Line Scale | 1011 | REAL | [VS:GetObjectVariableReal] |
| Design Text Scale | 1012 | REAL | [VS:GetObjectVariableReal] |
| Slash Thickness Scale | 1013 | REAL | [VS:GetObjectVariableReal] |
| Ambient light is ON | 1014 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Ambient Light Brightness | 1015 | REAL | [VS:GetObjectVariableReal] |
| HDRI Viewport | 1019 | LONGINT | [VS:GetObjectVariableLongInt] |
| 2D Class Attributes | 1020 | LONGINT | [VS:GetObjectVariableLongInt] |
| 2D Other Attributes | 1021 | LONGINT | [VS:GetObjectVariableLongInt] |
| 3D Class Fill Style | 1022 | LONGINT | [VS:GetObjectVariableLongInt] |
| 3D Class Line Style | 1023 | LONGINT | [VS:GetObjectVariableLongInt] |
| Viewport x Position | 1024 | REAL | [VS:GetObjectVariableReal] |
| Viewport y Position | 1025 | REAL | [VS:GetObjectVariableReal] |
| Angle With Axis | 1026 | REAL | [VS:GetObjectVariableReal] |
| Shadow Wall Components | 1027 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Gray Transparent | 1028 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Flip Text | 1029 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Black and White | 1030 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Viewport Use Document Class Visibility | 1031 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Viewport Description | 1032 | STRING value | [VS:GetObjectVariableString] |
| Viewport Locator | 1033 | STRING value | [VS:GetObjectVariableString] |
| Viewport Is Linked | 1032 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Viewport Display Planar | 1035 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Viewport Foreground Render Type | 1036 | INTEGER | [VS:GetObjectVariableInt] |

**Notes:**
1. View Type values are different then SetView

| viewUserDefined | 0 |
|-----------------|---|
| viewFront | 3 |
| viewBack | 4 |
| viewLeft | 5 |
| viewRight | 6 |
| viewTop | 7 |
| viewBottom | 8 |
| viewRightIso | 9 |
| viewLeftIso | 10 |
| viewRightRearIso | 11 |
| viewLeftRearIso | 12 |
| viewBottomRightIso | 13 |
| viewBottomLeftIso | 14 |
| viewBottomRightRearIso | 15 |
| viewBottomLeftRearIso | 16 |

## Walls

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Number of Cavities | 199 | INTEGER value (1) | [VS:GetObjectVariableInt] |
| Cavity is Pair | 240 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Cavity Fill Pattern | 260 | LONGINT index (0-71) (2) | [VS:GetObjectVariableLongInt] |
| Cavity Pen Weight | 280 | INTEGER value (mils) (2) | [VS:GetObjectVariableInt] |
| Cavity Pen Style | 300 | INTEGER index (2) | [VS:GetObjectVariableInt] |
| Cavity Left Offset | 320 | REAL (2) | [VS:GetObjectVariableReal] |
| Cavity Right Offset | 340 | REAL (2) | [VS:GetObjectVariableReal] |
| Hide Cavity Detail | 701 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Counterclockwise Round Wall | 570 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Round Wall Radius | 571 | REAL | [VS:GetObjectVariableReal] |
| Wall Left Gross Area | 608 | REAL | [VS:GetObjectVariableReal] |
| Wall Right Gross Area | 609 | REAL | [VS:GetObjectVariableReal] |
| Wall Gross Area | 610 | REAL | [VS:GetObjectVariableReal] |
| Wall Left Net Area | 611 | REAL | [VS:GetObjectVariableReal] |
| Wall Right Net Area | 612 | REAL | [VS:GetObjectVariableReal] |
| Wall Net Area | 613 | REAL | [VS:GetObjectVariableReal] |
| Wall Left Average Height | 614 | REAL | [VS:GetObjectVariableReal] |
| Wall Right Average Height | 615 | REAL | [VS:GetObjectVariableReal] |
| Wall Average Height | 616 | REAL | [VS:GetObjectVariableReal] |

**Notes:**
1. Pass NIL to access default cavity values.
2. To access different cavities within a wall, add the zero-based cavity index to the selector value. For example, to access the right offset of cavity 6, specify 346 (340 + 6).

## Wall and Slab Styles

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Thickness | 1177 | REAL (1) | [VS:GetObjectVariableReal] |
| Fill | 1178 | LONGINT Pattern (0 to 71) or negative resource fill ref number | [VS:GetObjectVariableLongInt] |
| Pen Style | 1179 | INTEGER Pattern (0 to 71) or dash (-1 to -10) | [VS:GetObjectVariableInt] |
| Pen Weight | 1180 | INTEGER | [VS:GetObjectVariableInt] |
| Fill Foreground Color | 1181 | INTEGER Color index (0 to 255) | [VS:GetObjectVariableInt] |
| Fill Background Color | 1182 | INTEGER Color index (0 to 255) | [VS:GetObjectVariableInt] |
| Pen Foreground Color | 1183 | INTEGER Color index (0 to 255) | [VS:GetObjectVariableInt] |
| Pen Background Color | 1184 | INTEGER Color index (0 to 255) | [VS:GetObjectVariableInt] |
| Opacity | 1185 | INTEGER Percent (0 to 100) | [VS:GetObjectVariableInt] |
| Use Fill Class Attributes | 1186 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Pen Class Attributes | 1187 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Use Class Opacity | 1188 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Cap Attributes Type | 1189 | INTEGER (0 = Wall line, 1 = Component lines) (2) | [VS:GetObjectVariableInt] |
| Caps | 1194 | INTEGER (0 = None, 1 = Start, 2 = End, 3 = Both) (2) | [VS:GetObjectVariableInt] |
| Class | 1195 | LONGINT Ref number | [VS:GetObjectVariableLongInt] |
| Control Offset | 1196 | REAL (2) | [VS:GetObjectVariableReal] |
| Texture Set | 1197 | INTEGER (0 = Object textures, 1 = Component textures) | [VS:GetObjectVariableInt] |
| Overall Texture | 1198 | LONGINT Ref number | [VS:GetObjectVariableLongInt] |
| Left Texture | 1199 | LONGINT Ref number (2) | [VS:GetObjectVariableLongInt] |
| Right Texture | 1200 | LONGINT Ref number (2) | [VS:GetObjectVariableLongInt] |
| Start Cap Texture | 1201 | LONGINT Ref number (2) | [VS:GetObjectVariableLongInt] |
| End Cap Texture | 1202 | LONGINT Ref number (2) | [VS:GetObjectVariableLongInt] |
| Top Texture | 1203 | LONGINT Ref number | [VS:GetObjectVariableLongInt] |
| Bottom Texture | 1204 | LONGINT Ref number | [VS:GetObjectVariableLongInt] |
| Holes Texture | 1205 | LONGINT Ref number (2) | [VS:GetObjectVariableLongInt] |
| Sides Texture | 1206 | LONGINT Ref number (3) | [VS:GetObjectVariableLongInt] |
| Mark | 1207 | STRING | [VS:GetObjectVariableString] |
| Description | 1208 | STRING | [VS:GetObjectVariableString] |
| Function | 1209 | STRING | [VS:GetObjectVariableString] |
| Exterior | 1210 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Load Bearing | 1211 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Fire Rating | 1212 | STRING | [VS:GetObjectVariableString] |
| Combustible Construction | 1213 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Compartmentation | 1214 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| U-Value | 1215 | REAL | [VS:GetObjectVariableReal] |
| R-Value | 1216 | REAL | [VS:GetObjectVariableReal] |
| Acoustic Rating | 1217 | STRING | [VS:GetObjectVariableString] |
| Cost Index System | 1218 | STRING | [VS:GetObjectVariableString] |
| Cost Index Code | 1219 | STRING | [VS:GetObjectVariableString] |
| Model | 1220 | STRING | [VS:GetObjectVariableString] |
| Manufacturer | 1221 | STRING | [VS:GetObjectVariableString] |
| URL | 1222 | STRING | [VS:GetObjectVariableString] |

**Notes:**
1. Wall Styles and read-only for Slab Styles
2. Wall Styles only
3. Slab Styles only

## Building Materials

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Is Volumetric | 1569 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Category | 1570 | STRING | [VS:GetObjectVariableString] |
| Standard | 1571 | INTEGER | [VS:GetObjectVariableInt] |
| | | 0 (Omni Class) | |
| | | 1 (Uni Class) | |
| | | 2 (None) | |
| | | 3 (Txt Class) | |
| Reference ID | 1572 | STRING | [VS:GetObjectVariableString] |
| Classification | 1573 | STRING | [VS:GetObjectVariableString] |
| Manufacturer | 1574 | STRING | [VS:GetObjectVariableString] |
| Product Model | 1575 | STRING | [VS:GetObjectVariableString] |
| Product Name | 1576 | STRING | [VS:GetObjectVariableString] |
| Product Description | 1577 | STRING | [VS:GetObjectVariableString] |
| Product URL | 1578 | STRING | [VS:GetObjectVariableString] |
| Specific Gravity | 1579 | REAL | [VS:GetObjectVariableReal] |
| Modulus of Elasticity | 1580 | REAL | [VS:GetObjectVariableReal] |
| Yield Strength | 1581 | REAL | [VS:GetObjectVariableReal] |
| Tensile Strength | 1582 | REAL | [VS:GetObjectVariableReal] |
| Specific Heat | 1583 | REAL | [VS:GetObjectVariableReal] |
| Emissivity | 1584 | REAL | [VS:GetObjectVariableReal] |
| Albedo | 1585 | REAL | [VS:GetObjectVariableReal] |
| Thermal Expansion Coefficient | 1586 | REAL | [VS:GetObjectVariableReal] |
| Lambda | 1587 | REAL | [VS:GetObjectVariableReal] |
| Embodied Carbon | 1588 | REAL | [VS:GetObjectVariableReal] |
| Sound Velocity | 1589 | REAL | [VS:GetObjectVariableReal] |
| Density | 1590 | REAL | [VS:GetObjectVariableReal] |
| Acoustic Impedance | 1591 | REAL | [VS:GetObjectVariableReal] |
| Uses Specific Gravity | 1592 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Modulus of Elasticity | 1593 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Yield Strength | 1594 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Tensile Strength | 1595 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Specific Heat | 1596 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Emissivity | 1597 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Albedo | 1598 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Thermal Expansion Coefficient | 1599 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Lambda | 1600 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Embodied Carbon | 1601 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Sound Velocity | 1602 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Density | 1603 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Uses Acoustic Impedance | 1604 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Is Surface Area Measure | 1605 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Description | 1606 | STRING | [VS:GetObjectVariableString] |
| Mark | 1607 | STRING | [VS:GetObjectVariableString] |
| Keynote | 1608 | STRING | [VS:GetObjectVariableString] |
| Cost | 1609 | STRING | [VS:GetObjectVariableString] |
| Source | 1610 | STRING | [VS:GetObjectVariableString] |
| Finish | 1611 | STRING | [VS:GetObjectVariableString] |
| Slip Resistance | 1612 | REAL | [VS:GetObjectVariableReal] |
| Uses Slip Resistance | 1613 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |

## Plug-in Objects

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Insertion Mode | 123 | 0 (On center of wall) | [VS:GetObjectVariableInt] |
| | | 1 (On edge of wall) | " |
| Break Mode | 124 | 1 (Full break) | [VS:GetObjectVariableInt] |
| | | 2 (Full break no caps) | " |
| | | 3 (Half break) | " |
| | | 4 (no break) | " |
| Font Style Enabled | 800 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| CreateCustomObject Don't Insert in Wall | 6709 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Parametric Internal ID | 1165 | INTEGER (read-only) | [VS:GetObjectVariableInt] |
| Parametric Localized Name | 1166 | STRING (read-only) | [VS:GetObjectVariableString] |
| Immediate Reset | 1167 | Write Only (Use on SDK parametric objects only!) | [VS:GetObjectVariableBoolean] |
| Hide Style Parameter check | 1168 | Read Only | [VS:GetObjectVariableBoolean] |

## 2D - 3D Status

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Object Is 3D | 650 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |
| Object Is 2D | 651 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |

## Worksheets

| Object Setting | Selector | Setting Value | Function |
|----------------|----------|---------------|----------|
| Worksheet Header | 80 | STRING value | [VS:GetObjectVariableString] |
| Worksheet Footer | 81 | STRING value | [VS:GetObjectVariableString] |
| Show Database Headers | 82 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Gridlines | 83 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Show Tabs | 84 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Auto-Recalculate | 85 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Default Font Index | 86 | INTEGER value | [VS:GetObjectVariableInt] |
| Default Font Size | 87 | INTEGER value | [VS:GetObjectVariableInt] |
| Top Print Margin | 88 | REAL value | [VS:GetObjectVariableReal] |
| Left Print Margin | 89 | REAL value | [VS:GetObjectVariableReal] |
| Bottom Print Margin | 90 | REAL value | [VS:GetObjectVariableReal] |
| Right Print Margin | 91 | REAL value | [VS:GetObjectVariableReal] |

## Textures

| Object Setting | Selector | Data Type | Function |
|----------------|----------|-----------|----------|
| Texturable Object | 500 | TRUE or FALSE (read-only) | [VS:GetObjectVariableBoolean] |
| Expanded Material Set | 501 | TRUE or FALSE (1) | [VS:GetObjectVariableBoolean] |
| Material Size | 511 | REAL (current units) | [VS:GetObjectVariableReal] |
| Texture Bitmap Horiz Repeat | 524 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Texture Bitmap Vertical Repeat | 525 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Texture Bitmap Feature Size | 527 | REAL (current units) | [VS:GetObjectVariableReal] |
| Paint Width | 530 | LONGINT (pixels) | [VS:GetObjectVariableInt] |
| Paint Height | 531 | LONGINT (pixels) | [VS:GetObjectVariableInt] |
| Texture Space Type | 540 | 0 (Plane) | [VS:GetObjectVariableInt] |
| | | 1 (Sphere) | " |
| | | 2 (Cylinder) | " |
| | | 3 (Algorithmic/Perimeter) | " |
| | | 4 (Shader) | " |
| Texture Space Scale | 543 | REAL | [VS:GetObjectVariableReal] |
| Texture Space Rotation | 544 | REAL value (in radians) | [VS:GetObjectVariableReal] |
| Texture Space Use Start Cap | 546 | TRUE or FALSE (3) | [VS:GetObjectVariableBoolean] |
| Texture Space Use End Cap | 547 | TRUE or FALSE (3) | [VS:GetObjectVariableBoolean] |
| Texture Space Part ID | 548 | INTEGER index (4) | [VS:GetObjectVariableInt] |
| Texture Space Radius | 549 | REAL (current units) (2) | [VS:GetObjectVariableReal] |
| Same Texture as Parent Wall | 704 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |

**Notes:**
1. Sets whether multiple textures can be applied to object (two for roof, three for walls).
2. Valid for sphere texture space only.
3. Valid for extrudes and sweeps only.
4. Index of multi-texturable object component.

## Gradient, Image, Tile and Hatch Fills

| Object Setting | Selector | Data Type | Function |
|----------------|----------|-----------|----------|
| Fill X Offset | 70 | REAL | [VS:GetObjectVariableReal] |
| Fill Y Offset | 71 | REAL | [VS:GetObjectVariableReal] |
| Fill I-Axis Length | 72 | REAL | [VS:GetObjectVariableReal] |
| Fill J-Axis Length | 73 | REAL | [VS:GetObjectVariableReal] |
| Fill Angle | 74 | REAL (radians) | [VS:GetObjectVariableReal] |
| Fill Repeat | 75 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Fill Mirror | 76 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Image Flip | 77 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Gradient Geometry Type | 78 | LONGINT | [VS:GetObjectVariableLongInt] |
| Image Aspect Ratio | 79 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Fill X Offset | 110 | REAL (current units) | [VS:GetObjectVariableReal] |
| Fill Y Offset | 111 | REAL (current units) | [VS:GetObjectVariableReal] |
| Fill I-Axis Length | 112 | REAL (current units) | [VS:GetObjectVariableReal] |
| Fill J-Axis Length | 113 | REAL (current units) | [VS:GetObjectVariableReal] |
| Image Width in Pixels | 534 | LONGINT | [VS:GetObjectVariableLongInt] |
| Image Width in Pixels | 535 | LONGINT | [VS:GetObjectVariableLongInt] |

## Hatches

| Object Setting | Selector | Data Type | Function |
|----------------|----------|-----------|----------|
| Number of Levels | 660 | INTEGER | [VS:GetObjectVariableInt] |
| Is Transparent | 661 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Has Page Units | 662 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Rotate In Wall | 663 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Rotate In Symbol | 664 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |

## Materials

Selectors are here: [VS:Working_with_Materials](VS:Working_with_Materials#MaterialProperty_values)

## Misc.

| Object Setting | Selector | Data Type | Function |
|----------------|----------|-----------|----------|
| Is 2D Poly Clockwise | 652 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Object Fill Style | 695 | LONGINT | [VS:GetObjectVariableLongInt] |
| Object Fill Type | 696 | INTEGER | [VS:GetObjectVariableInt] |
| Object Use Local Mapping | 697 | BOOLEAN | [VS:GetObjectVariableBoolean] |
| Object is Locked | 700 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Object is visible in high detail level | 750 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Object is visible in middle detail level | 751 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Object is visible in low detail level | 752 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Format is Visible | 900 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Text Is Linked To Record | 680 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Text Repeating Tab | 682 | REAL (current units) | [VS:GetObjectVariableReal] |
| Sweep Z Offset | 401 | REAL (current units) | [VS:GetObjectVariableReal] |
| Saved View Saves View Orientation | 450 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Saved View Saves Zoom and Pan | 456 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Saved View Saves Page Location | 451 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Saved View Saves Class Visibilities | 452 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Saved View Saves Layer Visibilities | 453 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Solid Has History | 630 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Solid Scale X | 631 | REAL scale factor | [VS:GetObjectVariableReal] |
| Solid Scale Y | 632 | REAL scale factor | [VS:GetObjectVariableReal] |
| Solid Scale Z | 633 | REAL scale factor | [VS:GetObjectVariableReal] |
| Bitmap Object Compression | 532 | 0 (None) | [VS:GetObjectVariableLongInt] |
| | | 1 (JPEG) | " |
| | | 2 (PNG) | " |
| | | 3 (PNG Monochrome) | " |
| Image Resource Compression | 533 | 0 (None) | [VS:GetObjectVariableLongInt] |
| | | 1 (JPEG) | " |
| | | 2 (PNG) | " |
| | | 3 (PNG Monochrome) | " |
| Set Specified Design Layer Visibility in All Saved Views | 454 | -1 (Invisible) | [VS:GetObjectVariableInt] |
| | | 0 (Normal) | " |
| | | 2 (Grayed) | " |
| | | 3 (Don't Save) | " |
| Set Specified Class Visibility in All Saved Views | 455 | -1 (Invisible) | [VS:GetObjectVariableInt] |
| | | 0 (Normal) | " |
| | | 2 (Grayed) | " |
| | | 3 (Don't Save) | " |
| Mark Object as Structural | 702 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| First Aux List Object | 703 | HANDLE | [VS:GetObjectVariableHandle] |
| Custom Object Area | 801 | REAL (current units) | [VS:GetObjectVariableReal] |
| Custom Object Perimeter | 802 | REAL (current units) | |
| Sketch Style | 1100 | -2 No Sketch | [VS:GetObjectVariableLongInt] |
| | | 0 Default | |
| | | Index of Sketch Style | |
| Set Specified Design Layer Visibility In All Viewports | 1017 | INTEGER | [VS:GetObjectVariableInt] |
| Set Specified Class Visibility In All Viewports | 1018 | INTEGER | [VS:GetObjectVariableInt] |
| Projection Type | 1110 | 0 (Lambert Conic) 1 (UTM) | [VS:GetObjectVariableInt] |
| Lat./Long. vs XY Flag | 1111 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| First Import Flag | 1112 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| New Layer/Class Flag | 1113 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
| Model Space Scale | 1114 | REAL | [VS:GetObjectVariableReal] |
| Georeference Point | 1115 | REAL | [VS:GetObjectVariableReal] |
| Georeference Offset | 1116 | REAL | [VS:GetObjectVariableReal] |
| Layer of First Import To Class | 1117 | LONGINT | [VS:GetObjectVariableLongInt] |
| Thumbnail View | 1152 | INTEGER | [VS:GetObjectVariableInt] |
| Thumbnail Render | 1153 | INTEGER | [VS:GetObjectVariableInt] |
| RenderWorks Background Width | 1154 | REAL (current units) | [VS:GetObjectVariableReal] |
| RenderWorks Background Height | 1155 | REAL (current units) | [VS:GetObjectVariableReal] |
| Planar Object Is Screen Object | 1160 | TRUE or FALSE | [VS:GetObjectVariableBoolean] |
