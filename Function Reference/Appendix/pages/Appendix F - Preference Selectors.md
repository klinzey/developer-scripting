# Appendix F - Preference Selectors

## Application Preference Selectors

| Preference | Selector | Preference Value | Function |
|------------|----------|------------------|----------|
| Click-Drag Mode | 0 | TRUE or FALSE | [[VS:GetPref]] |
| Offset Duplicates | 1 | TRUE or FALSE | [[VS:GetPref]] |
| Full Screen Cursor | 2 | TRUE or FALSE | [[VS:GetPref]] |
| Show Screen Hints | 3 | TRUE or FALSE | [[VS:GetPref]] |
| Floating Datum | 4 | TRUE or FALSE | [[VS:GetPref]] |
| Snap To Loci | 5 | TRUE or FALSE | [[VS:GetPref]] |
| Show Rulers | 6 | TRUE or FALSE | [[VS:GetPref]] |
| Show Scroll Bars | 7 | TRUE or FALSE | [[VS:GetPref]] |
| No Fill Behind Text | 8 | TRUE or FALSE | [[VS:GetPref]] |
| Zoom Line Thickness | 9 | TRUE or FALSE | [[VS:GetPref]] |
| Black and White Only | 10 | TRUE or FALSE | [[VS:GetPref]] |
| Use Layer Colors | 11 | TRUE or FALSE | [[VS:GetPref]] |
| Log Time in Program | 12 | TRUE or FALSE | [[VS:GetPref]] |
| Adjust Flipped Text | 13 | TRUE or FALSE | [[VS:GetPref]] |
| Show Other Objects While In Group | 14 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Axis Labels | 15 | TRUE or FALSE | [[VS:GetPref]] |
| Use Black Background | 16 | TRUE or FALSE | [[VS:GetPref]] |
| Use Eight Selection Handles | 17 | TRUE or FALSE | [[VS:GetPref]] |
| Current Background Color | 4003 | | [[vs:GetPrefRGB]] |
| Use Sound | 18 | TRUE or FALSE | [[VS:GetPref]] |
| Issue Undo Warnings | 19 | TRUE or FALSE | [[VS:GetPref]] |
| Opaque SmartCursor | 20 | TRUE or FALSE | [[VS:GetPref]] |
| Stop VectorScript on Warnings | 21 | TRUE or FALSE | [[VS:GetPref]] |
| Left Palette Margin | 22 | TRUE or FALSE | [[VS:GetPref]] |
| Right Palette Margin | 23 | TRUE or FALSE | [[VS:GetPref]] |
| Use Save Reminder | 24 | TRUE or FALSE | [[VS:GetPref]] |
| Show Parametric Constraints | 25 | TRUE or FALSE | [[VS:GetPref]] |
| Display Minor Alerts on Mode Bar | 27 | TRUE or FALSE | [[VS:GetPref]] |
| Associate Dimensions | 28 | TRUE or FALSE | [[VS:GetPref]] |
| Spell Check Capitalized Words | 29 | TRUE or FALSE | [[VS:GetPref]] |
| Spell Check Words in ALL CAPS | 30 | TRUE or FALSE | [[VS:GetPref]] |
| Spell Check Mixed Case Words | 31 | TRUE or FALSE | [[VS:GetPref]] |
| Spell Check Words With Numbers | 32 | TRUE or FALSE | [[VS:GetPref]] |
| Auto Join Walls | 33 | TRUE or FALSE | [[VS:GetPref]] |
| Show Page Breaks | 34 | TRUE or FALSE | [[VS:GetPref]] |
| Show Grid | 35 | TRUE or FALSE | [[VS:GetPref]] |
| Print Grid | 36 | TRUE or FALSE | [[VS:GetPref]] |
| Snap To Grid | 37 | TRUE or FALSE | [[VS:GetPref]] |
| Snap To Object | 38 | TRUE or FALSE | [[VS:GetPref]] |
| Use Occluded Picking And Snapping | 105 | TRUE or FALSE | [[VS:GetPref]] |
| Save By Time | 39 | TRUE or FALSE | [[VS:GetPref]] |
| Save Confirm | 40 | TRUE or FALSE | [[VS:GetPref]] |
| Save To Backup | 41 | TRUE or FALSE | [[VS:GetPref]] |
| Palette Docking | 43 | TRUE or FALSE | [[VS:GetPref]] |
| Create Dimensions in Dimension Class | 44 | TRUE or FALSE | [[VS:GetPref]] |
| Accelerated 2D Navigation | 45 | TRUE or FALSE | [[VS:GetPref]] |
| Use Vector Caching | 46 | TRUE or FALSE | [[VS:GetPref]] |
| Sketch Hidden Line | 47 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Edge Points | 48 | TRUE or FALSE | [[VS:GetPref]] |
| Show Page Boundary | 49 | TRUE or FALSE | [[VS:GetPref]] |
| Display Default Content | 130 | TRUE or FALSE | [[VS:GetPref]] |
| Dimension Slash Thickness Unit | 50 | 3 = points, 2 = mils, 1 = mm | [[VS:GetPrefInt]] |
| 3D Rotation Responsiveness | 52 | 1(detailed)..5(responsive) | [[VS:GetPrefInt]] |
| Custom Constraint Angle | 53 | REAL (degrees) | [[VS:GetPrefReal]] |
| Snap Radius | 54 | INTEGER value | [[VS:GetPrefInt]] |
| 2D Conversion Resolution | 55 | INTEGER value | [[VS:GetPrefInt]] |
| 3D Conversion Resolution | 56 | INTEGER value | [[VS:GetPrefInt]] |
| Current Document Text Size | 57 | REAL | [[VS:GetPrefReal]] |
| Current Document Text Style | 58 | 0 (Plain) | [[VS:GetPrefInt]] |
| | | 1 (Bold) | |
| | | 2 (Italic) | |
| | | 4 (Underline) | |
| | | 8 (Outline [Mac only]) | |
| | | 16 (Shadow [Mac only]) | |
| Current Document Text Justification | 82 | 1 (Left) | [[VS:GetPrefInt]] |
| | | 2 (Center) | |
| | | 3 (Right) | |
| Current Document Text Vertical Alignment | 83 | 1 (TopBox) | [[VS:GetPrefInt]] |
| | | 2 (TopBaseline) | |
| | | 3 (CenterBox) | |
| | | 4 (BottomBaseline) | |
| | | 5 (BottomBox) | |
| Current Document Text Vertical Spacing | 84 | 0 (Custom Leading) | [[VS:GetPrefInt]] |
| | | 2 (Single) | |
| | | 3 (Three Halves) | |
| | | 4 (Double) | |
| Current Document Text Vertical Spacing Custom Value | 85 | REAL | [[VS:GetPrefReal]] |
| Maximum Number of Undos | 59 | INTEGER | [[VS:GetPrefInt]] |
| Undo View Changes | 26 | 1 (never) | [[VS:GetPrefInt]] |
| | | 2 (combine all) | |
| | | 3 (combine similar) | |
| | | 4 (combine none) | |
| Save Interval | 60 | no. of minutes | [[VS:GetPrefInt]] |
| Display Light Objects | 61 | 0(always) | [[VS:GetPrefInt]] |
| | | 1(wireframe) | |
| | | 2(never) | |
| Display 3D Loci Objects | 91 | 0(always) | [[VS:GetPrefInt]] |
| | | 1(wireframe) | |
| | | 2(never) | |
| Retain QuickDraw 3D Model | 62 | 1(never)...5(always) | [[VS:GetPrefInt]] |
| Rotated Text Display | 63 | 0(box) | [[VS:GetPrefInt]] |
| | | 1(normal) | |
| | | 2(high) | |
| Bitmap Display | 64 | 0(box) | [[VS:GetPrefInt]] |
| | | 1(low res) | |
| | | 2(hi res) | |
| Dimension Slash Thickness | 65 | INTEGER value (mils) | [[VS:GetPrefInt]] |
| Hidden Line Dash Style | 197 | LONGINT selector | [[VS:GetPrefLongInt]] |
| Hidden Line Shading | 67 | 1(dark)...4(light) | [[VS:GetPrefInt]] |
| Grid X | 78 | REAL | [[VS:GetPrefReal]] |
| Grid Y | 79 | REAL | [[VS:GetPrefReal]] |
| User Origin X | 6702 | REAL (current units) | [[VS:GetPrefReal]] |
| User Origin Y | 6702 | REAL (current units) | [[VS:GetPrefReal]] |
| Page Origin X | 80 | REAL (current units) | [[VS:GetPrefReal]] |
| Page Origin Y | 81 | REAL (current units) | [[VS:GetPrefReal]] |
| Page Scaling Factor | 70 | REAL | [[VS:GetPrefReal]] |
| Dimension Standard | 71 | 1 (Arch) | [[VS:GetPrefInt]] |
| | | 2 (ASME) | |
| | | 3 (BSI) | |
| | | 4 (DIN) | |
| | | 5 (ISO) | |
| | | 6 (JIS) | |
| | | 7 (SIA) | |
| | | 8 (ASME Dual Side-by-Side) | |
| | | 9 (ASME Dual Stacked) | |
| Defacet Angle | 72 | REAL (0-90) | [[VS:GetPrefReal]] |
| Grid Angle | 73 | REAL | [[VS:GetPrefReal]] |
| Move Objects on Grid Keys | 74 | 1 (arrow) | [[VS:GetPrefInt]] |
| | | 2 (cmd+arrow) | |
| | | 3 (shift+arrow) | |
| | | 4 (shift+cmd+arrow) | |
| Nudge Objects Keys | 75 | 1-4 (see above) | [[VS:GetPrefInt]] |
| Show Nudge Message | 6712 | TRUE or FALSE | [[VS:GetPref]] |
| Pan Drawing Keys | 76 | 1-4 (see above) | [[VS:GetPrefInt]] |
| Switch Active Layer/Class Keys | 77 | 1-4 (see above) | [[VS:GetPrefInt]] |
| Default Compression | 86 | 1 = JPEG, 2 = PNG | [[VS:GetPrefInt]] |
| Line Weight Array Count | 87 | INTEGER | [[VS:GetPrefInt]] |
| Sound Volume | 88 | INTEGER | [[VS:GetPrefInt]] |
| Custom Move Distance | 89 | REAL | [[VS:GetPrefReal]] |
| Plan Rotation | 92 | TRUE or FALSE | [[VS:GetPref]] |
| Plan Rotation Angle | 93 | REAL (read-only) | [[VS:GetPrefReal]] |
| Stack Layers | 94 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Create 2D Objects | 95 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Ignore Other Scales | 96 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Restore Views | 97 | TRUE or FALSE | [[VS:GetPref]] |
| Use Open MP Multithreading | 98 | 0 (No) | [[VS:GetPrefInt]] |
| | | 1 (Yes) | |
| | | 2 (Partial) | |
| Stack Layers Center View | 99 | TRUE or FALSE | [[VS:GetPref]] |
| Text Font Name | 100 | STRING | [[VS:GetPrefString]] |
| Stack Layers Show Page Boundary | 101 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Only Active Layer 2D Objects | 102 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Display Only Story Layers | 103 | TRUE or FALSE | [[VS:GetPref]] |
| Stack Layers Stories Enabled | 104 | TRUE or FALSE | [[VS:GetPref]] |
| Enable Legacy 2D Layer Mode | 6839 | TRUE or FALSE | [[VS:GetPref]] |
| Angular Precision | 120 | INTEGER | [[VS:GetPrefInt]] |
| Angular Unit | 121 | 0 (degrees) | [[VS:GetPrefInt]] |
| | | 1 (radians) | |
| | | 2 (gradians) | |
| Resetting Plugin-ins During File Read | 129 | TRUE or FALSE | [[VS:GetPref]] |
| Enable Vectorworks Libraries | 130 | TRUE or FALSE | [[VS:GetPref]] |
| Auto File Extensions On Mac | 131 | TRUE or FALSE | [[VS:GetPref]] |
| Use Advanced Imaging | 132 | TRUE or FALSE | [[VS:GetPref]] |
| Use Anti Aliasing | 133 | TRUE or FALSE | [[VS:GetPref]] |
| Auto Associate Dims | 134 | TRUE or FALSE | [[VS:GetPref]] |
| Mouse Wheel Zoom | 135 | TRUE or FALSE | [[VS:GetPref]] |
| Use Custom Move Distance | 136 | TRUE or FALSE | [[VS:GetPref]] |
| Print Switch Binary | 137 | TRUE or FALSE | [[VS:GetPref]] |
| Create New Document on Startup | 138 | TRUE or FALSE | [[VS:GetPref]] |
| Change Layer for Create Similar | 139 | TRUE or FALSE | [[VS:GetPref]] |
| Show Watermarks | 142 | TRUE or FALSE | [[VS:GetPref]] |
| Unit1 Dim Fraction Display Style | 190 | 0 (regular style) | [[VS:GetPrefInt]] |
| | | 1 (diagonal style) | |
| | | 2 (horizontal style) | |
| DXF Add Prefix To DXF Layers | 328 | TRUE or FALSE | [[VS:GetPref]] |
| DXF Prefix To DXF Edit | 329 | STRING value | [[VS:GetPrefString]] |
| DXF External Refs Handling | 330 | 0 (Bind External Refs) | [[VS:GetPrefInt]] |
| | | 1 (Ignore External Refs) | |
| | | 2 (Create VW Refs) | |
| | | 3 (Use Layer Import) | |
| DXF ADT Objects 2D View | 331 | TRUE or FALSE | [[VS:GetPref]] |
| Use Framed Highlighting | 410 | TRUE or FALSE | [[VS:GetPref]] |
| Smart Cursor Show Interactive Segment | 411 | TRUE or FALSE | [[VS:GetPref]] |
| Snap To Tool Snap Geometry Only | 460 | TRUE or FALSE | [[VS:GetPref]] |
| whether to coordinate sheet and drawing numbers for various items | 544 | TRUE or FALSE | [[VS:GetPref]] |
| Auto Save To Custom Location | 552 | TRUE or FALSE | [[VS:GetPref]] |
| Autosave Custom Location | 554 | STRING value | [[VS:GetPrefString]] |
| Keep Backups By Number Value | 555 | TRUE or FALSE | [[VS:GetPref]] |
| Center View | 558 | TRUE or FALSE | [[VS:GetPref]] |
| Allow Copy on Option Click | 559 | TRUE or FALSE | [[VS:GetPref]] |
| AutoUpdate Frequency | 1054 | INTEGER | [[VS:GetPrefInt]] |
| Error Reporting Mode | 1056 | INTEGER | [[VS:GetPrefInt]] |
| Use Multithreading for Textures | 1057 | TRUE or FALSE | [[VS:GetPref]] |
| Use Multithreading for Image | 1058 | TRUE or FALSE | [[VS:GetPref]] |
| Use Multithreading for Render | 1059 | TRUE or FALSE | [[VS:GetPref]] |
| Use Multithreading for Geometry | 1060 | TRUE or FALSE | [[VS:GetPref]] |
| Use Multithreading for DTM | 1061 | TRUE or FALSE | [[VS:GetPref]] |
| Use Multithreading for Other | 1062 | TRUE or FALSE | [[VS:GetPref]] |
| Use Open MP Multithreading | 98 | 0 = No | [[VS:GetPrefInt]] |
| | | 1 = Yes | |
| | | 2 = Partial | |
| Save DTM Cache | 1097 | TRUE or FALSE | [[VS:GetPref]] |
| Enable X-Ray Mode | 106 | TRUE or FALSE | [[VS:GetPref]] |
| Scale Layer Text | 107 | TRUE or FALSE | [[VS:GetPref]] |
| Hierarchical Classes In Popups | 108 | TRUE or FALSE | [[VS:GetPref]] |
| Save Expand State Of Classes In Popups | 111 | TRUE or FALSE | [[VS:GetPref]] |
| Save Undo View Changes | 112 | TRUE or FALSE | [[VS:GetPref]] |
| Fill Style By Class | 534 | TRUE or FALSE | [[VS:GetPref]] |
| Setting low detail factor. If LayerScales >= LowDetailFactor will only show low detail and will hide wall cavities | 538 | REAL | [[VS:GetPrefReal]] |
| Setting medium detail factor. LayerScales >= MediumDetailFactor will show medium detail, <= MediumDetailFactor will show high detail | 539 | REAL | [[VS:GetPrefReal]] |
| View Transition Animation | 1227 | TRUE or FALSE | [[VS:GetPref]] |
| View Transition Speed | 6725 | Real | [[VS:GetPref]] |
| Allow Docking to Drawing | 6752 | TRUE or FALSE | [[VS:GetPref]] |
| Allow Internal Palette Docking | 6753 | TRUE or FALSE | [[VS:GetPref]] |
| Show Docked Document Tabs | 6754 | TRUE or FALSE | [[VS:GetPref]] |
| Force the tool to trap the shift key for when it is used with the short keys for modebar | 6770 | TRUE or FALSE (write only) | [[VS:GetPref]] |
| Controls the state in which windowshaded palettes automaticaly unshade based on mouse proximity | 6775 | TRUE or FALSE | [[VS:GetPref]] |
| Controls the state in which docked palettes automaticaly hides based on mouse proximity | 6776 | TRUE or FALSE | [[VS:GetPref]] |
| Worksheet parameter delimiter | 6798 | String | [[VS:GetPrefString]] |
| Turns screen redraws on/off | 6799 | Boolean | [[VS:GetPref]] |
| Enable Multiview | 6802 | Boolean | [[VS:GetPref]] |
| Multiview visibilities | 6803 | Boolean | [[VS:GetPref]] |
| turns on/off the Duplicate Tags With Objects | 6804 | [[VS:GetPref]] |
| turns on/off the drawing of the ray+octree intersected mesh vrefs | 6806 | Boolean | [[VS:GetPref]] |
| Enable profile VectorScript execution | 6807 | Boolean | [[VS:GetPref]] |
| Enable profile VectorScript execution | 6807 | Boolean | [[VS:GetPref]] |
| Enable On Demand Level Of Detail | 6808 | Boolean | [[VS:GetPref]] |
| Hide GPU Display Alert Dialog | 6809 | Boolean | [[VS:GetPref]] |
| Hide Graphics Adapters Alert Dialog | 6810 | Boolean | [[VS:GetPref]] |
| Enable OnDemand Level Of Detail 2D | 6811 | Boolean | [[VS:GetPref]] |
| Smart Cursor Lock Special X | 6812 | REAL | [[VS:GetPrefReal]] |
| Smart Cursor Lock Special Y | 6813 | REAL | [[VS:GetPrefReal]] |
| Use OpenGL Background Supported | 6816 | Boolean | [[VS:GetPref]] |
| OpenGL AntiAliasing Supported | 593 | Boolean | [[VS:GetPref]] |
| OpenGL Draw Edges Supported | 594 | Boolean | [[VS:GetPref]] |
| OpenGL Use Shadows Supported | 595 | Boolean | [[VS:GetPref]] |
| Block Until Done Rendering | 596 | Boolean (write only) | [[VS:GetPref]] |
| Allow Drop Shadows | 597 | Boolean | [[VS:GetPref]] |
| OpenGL Environment Lighting Capability | 598 | Boolean | [[VS:GetPref]] |
| OpenGL Environment Reflection Capability | 599 | Boolean | [[VS:GetPref]] |
| OpenGL Screen Space Reflection Capability | 601 | Boolean | [[VS:GetPref]] |
| Dark Sym Previews | 602 | Boolean | [[VS:GetPref]] |
| Use Duplicates For Raster VPs | 6817 | Boolean | [[VS:GetPref]] |
| Default Render Mode Render Mode | 1318 | INTEGER | [[VS:GetPrefInt]] |
| Default Render Mode Projection Mode | 1319 | INTEGER | [[VS:GetPrefInt]] |
| Use Local Help System | 6724 | TRUE or FALSE | [[VS:GetPref]] |
| Display Home Screen on Startup | 7009 | TRUE or FALSE | [[VS:GetPref]] |
| Display Home Screen on Closing Last Doc | 7010 | TRUE or FALSE | [[VS:GetPref]] |
| Enable Legacy Eight Lights | 7100 | TRUE or FALSE | [[VS:GetPref]] |
| Display Non-Printable Indicators | 7301 | TRUE or FALSE | [[VS:GetPref]] |
| Release Version Integer | 570 | SHORT - The release version integer defaults to 0 | [[VS:GetPrefInt]] |
| get/set the insertion mode of the symbol tool | 580 | SHORT | [[VS:GetPrefInt]] |
| get/set the wall insertion mode of the symbol tool | 581 | SHORT | [[VS:GetPrefInt]] |
| get/set the alignment mode of the symbol tool | 582 | SHORT | [[VS:GetPrefInt]] |
| Parametric Enable State Eventing | 590 | 0 (NoStateEvents) | [[VS:GetPrefInt]] |
| | | 1 (ResetStatesEvent) | [[VS:GetPrefInt]] |
| | | 2 (InternalStatesEvent) | [[VS:GetPrefInt]] |

### Smart Cursor / Appearance Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Store / Recall Interactive Preferences | 1200 | Set=Store Get=Recall | [[VS:GetPref]] |
| Show Selection Box | 1000 | TRUE or FALSE | [[VS:GetPref]] |
| Show Snap Box | 1001 | TRUE or FALSE | [[VS:GetPref]] |
| Animation Mode | 1003 | INTEGER | [[VS:GetPrefInt]] |
| Pre-selection Highlighting | 1004 | TRUE or FALSE | [[VS:GetPref]] |
| Marquee Pre-selection Highlighting | 1005 | TRUE or FALSE | [[VS:GetPref]] |
| Snapped Object Pre-selection Highlighting | 1006 | TRUE or FALSE | [[VS:GetPref]] |
| Tool Highlighting | 1007 | TRUE or FALSE | [[VS:GetPref]] |
| Highlighting Timer | 1008 | REAL | [[VS:GetPrefReal]] |
| Selection Radius | 1009 | REAL | [[VS:GetPrefReal]] |
| Snap Box Radius | 1010 | REAL | [[VS:GetPrefReal]] |
| Show Snap Points | 1013 | TRUE or FALSE | [[VS:GetPref]] |
| Zoom to Linethickness in Snap Loop | 1014 | TRUE or FALSE | [[VS:GetPref]] |
| Offset from Source | 1015 | TRUE or FALSE | [[VS:GetPref]] |
| Show Acquisition Hints | 1016 | TRUE or FALSE | [[VS:GetPref]] |
| Reference Grid X | 1019 | REAL | [[VS:GetPrefReal]] |
| Reference Grid Y | 1020 | REAL | [[VS:GetPrefReal]] |
| Grid Angle Y | 1021 | REAL | [[VS:GetPrefReal]] |
| Sheet Layer Grid Snap X | 1022 | REAL | [[VS:GetPrefReal]] |
| Sheet Layer Grid Snap Y | 1023 | REAL | [[VS:GetPrefReal]] |
| Sheet Layer Reference Grid X | 1024 | REAL | [[VS:GetPrefReal]] |
| Sheet Layer Reference Grid Y | 1025 | REAL | [[VS:GetPrefReal]] |
| Sheet Layer Grid Angle Y | 1026 | REAL | [[VS:GetPrefReal]] |
| Snap to End Point | 1027 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Mid Point | 1028 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Center Point | 1029 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Quadrant Points | 1030 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Insertion Point | 1031 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Vertex Points | 1032 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Nearest point on Edge | 1033 | TRUE or FALSE | [[VS:GetPref]] |
| Snap Angles in Degrees | 1034 | Angles are separated by a Semicolon | [[VS:GetPrefString]] |
| Plan Rotation | 1035 | TRUE or FALSE | [[VS:GetPref]] |
| Show Alternate Cordinate Extension Lines | 1036 | TRUE or FALSE | [[VS:GetPref]] |
| Show Horizontal Vertical Extensions | 1037 | TRUE or FALSE | [[VS:GetPref]] |
| Use Angular Extensions | 1038 | TRUE or FALSE | [[VS:GetPref]] |
| Use Floating Smart Point | 1039 | TRUE or FALSE | [[VS:GetPref]] |
| Acquire Smart Point if the mouse stops for | 1040 | REAL | [[VS:GetPrefReal]] |
| Set Datum if mouse stops for | 1041 | REAL | [[VS:GetPrefReal]] |
| Use Datum Offset | 1042 | TRUE or FALSE | [[VS:GetPref]] |
| Datum Offset | 1043 | REAL | [[VS:GetPrefReal]] |
| Acquire Edge | 1044 | TRUE or FALSE | [[VS:GetPref]] |
| Acquire Edge if mouse follows edge for | 1045 | REAL | [[VS:GetPrefReal]] |
| Snap to Bisector | 1046 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Offset | 1047 | TRUE or FALSE | [[VS:GetPref]] |
| Snap Offset Diatance | 1048 | REAL | [[VS:GetPrefReal]] |
| Snap to Extension Lines | 1049 | TRUE or FALSE | [[VS:GetPref]] |
| Snap Proportional | 1050 | TRUE or FALSE | [[VS:GetPref]] |
| Snap by Percent | 1051 | REAL | [[VS:GetPrefReal]] |
| Snap by Distance | 1052 | REAL | [[VS:GetPrefReal]] |
| Snap Mutiple Divisions | 1053 | TRUE or FALSE | [[VS:GetPref]] |
| Show Others in Group Gray | 1055 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Z Axis | 1063 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Z Axis Grp | 1064 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Relative Angles | 1086 | TRUE or FALSE | [[VS:GetPref]] |
| Relative Snap Angle | 1087 | Clockwise from Horizontal | [[VS:GetPrefReal]] |
| Relative Snap Angle Hint | 1088 | TRUE = Tangent FALSE = Parallel | [[VS:GetPref]] |
| Clear Relative Angle and Hint | 1089 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Combined Page Area | 1090 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Individual Pages | 1091 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Angles form Axes | 1092 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Alternate Cordinate System | 1093 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Line Between Smart Points | 1094 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to All Extensions from Nearby Smart Points | 1095 | TRUE or FALSE | [[VS:GetPref]] |
| Disable All Snaps | 1096 | TRUE or FALSE | [[VS:GetPref]] |
| Show Working Plane Axes in Plan View | 1098 | TRUE or FALSE | [[VS:GetPref]] |

### Interactive Smart Cursor Dialog Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Store / Recall Interactive Preferences | 1200 | Set=Store Get=Recall | [[VS:GetPref]] |
| Full Screen Cursor | 1210 | TRUE or FALSE | [[VS:GetPref]] |
| Show Selection Box | 1211 | TRUE or FALSE | [[VS:GetPref]] |
| Show Snap Box | 1212 | TRUE or FALSE | [[VS:GetPref]] |
| Show Acquisition Hints | 1213 | TRUE or FALSE | [[VS:GetPref]] |
| Selection Radius | 1214 | Screen Inches | [[VS:GetPrefReal]] |
| Snap Radius | 1215 | Screen Inches | [[VS:GetPrefReal]] |
| Grid Radius | 1216 | Screen Inches | [[VS:GetPrefReal]] |
| Selection Highlighting Mode | 1220 | | [[VS:GetPrefInt]] |
| Animation Mode | 1221 | | [[VS:GetPrefInt]] |
| Cursor Preselection Highlighting | 1222 | TRUE or FALSE | [[VS:GetPref]] |
| Marquee Preselection Highlighting | 1223 | TRUE or FALSE | [[VS:GetPref]] |
| Snapped Object Highlighting | 1224 | TRUE or FALSE | [[VS:GetPref]] |
| Tool Highlighting | 1225 | TRUE or FALSE | [[VS:GetPref]] |
| Highlighting Timer | 1226 | | [[VS:GetPrefReal]] |
| Show Smart Cursor Cues | 1230 | TRUE or FALSE | [[VS:GetPref]] |
| Show Snap Points | 1231 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Loci | 1232 | TRUE or FALSE | [[VS:GetPref]] |
| Zoom Line Thickness in Snap Loop | 1233 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Combined Page Area | 1234 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Individual Pages | 1235 | TRUE or FALSE | [[VS:GetPref]] |
| Offset from Source | 1236 | TRUE or FALSE | [[VS:GetPref]] |
| Ignore Non Planar Shapes | 1237 | TRUE or FALSE | [[VS:GetPref]] |
| Do Not Show Grid | 1240 | TRUE or FALSE | [[VS:GetPref]] |
| Print Grid | 1241 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Axis Grid | 1242 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Axis Grid Labels | 1243 | TRUE or FALSE | [[VS:GetPref]] |
| Show 3D Axis Grid Grip | 1299 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to End Points | 1250 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Mid Point | 1251 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Center | 1252 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Quad | 1253 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Intersection | 1254 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Vertex | 1255 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Edge | 1256 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Master | 1257 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to User Angles | 1260 | TRUE or FALSE | [[VS:GetPref]] |
| User Angle Count | 1261 | 1 to 8 | [[VS:GetPrefInt]] |
| User Angle Degrees 1 | 1262 | | [[VS:GetPrefReal]] |
| User Angle Degrees 2 | 1263 | | [[VS:GetPrefReal]] |
| User Angle Degrees 3 | 1264 | | [[VS:GetPrefReal]] |
| User Angle Degrees 4 | 1265 | | [[VS:GetPrefReal]] |
| User Angle Degrees 5 | 1266 | | [[VS:GetPrefReal]] |
| User Angle Degrees 6 | 1267 | | [[VS:GetPrefReal]] |
| User Angle Degrees 7 | 1268 | | [[VS:GetPrefReal]] |
| User Angle Degrees 8 | 1269 | | [[VS:GetPrefReal]] |
| Snap to Relative Angles | 1280 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Plan Rotation Angle | 1281 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Alternative Coordinate System | 1282 | TRUE or FALSE | [[VS:GetPref]] |
| Alternative Coordinate System Angle | 1283 | | [[VS:GetPrefReal]] |
| Use Horizontal and Vertical Extensions | 1290 | TRUE or FALSE | [[VS:GetPref]] |
| Use Angular Extensions | 1291 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Lines Between Smart Points | 1292 | TRUE or FALSE | [[VS:GetPref]] |
| Allow Extensions from Nearby Smart Points | 1293 | TRUE or FALSE | [[VS:GetPref]] |
| Use Floating Smart Points | 1294 | TRUE or FALSE | [[VS:GetPref]] |
| Floating Point Smart Time | 1295 | Seconds | [[VS:GetPrefReal]] |
| Use Floating Datum | 1296 | TRUE or FALSE | [[VS:GetPref]] |
| Floating Datum Time | 1297 | Seconds | [[VS:GetPrefReal]] |
| Use Floating Edges | 1300 | TRUE or FALSE | [[VS:GetPref]] |
| Floating Edge Time | 1301 | Seconds | [[VS:GetPrefReal]] |
| Use Angle Bisector | 1302 | TRUE or FALSE | [[VS:GetPrefReal]] |
| Use Curve Extensions | 1303 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Object | 1310 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Grid | 1311 | TRUE or FALSE | [[VS:GetPref]] |
| Constrain to Angle | 1312 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Intersection | 1313 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Smart Points | 1314 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Distance | 1315 | TRUE or FALSE | [[VS:GetPref]] |
| Snap to Smart Edge | 1316 | TRUE or FALSE | [[VS:GetPref]] |
| Constrain Tangent | 1317 | TRUE or FALSE | [[VS:GetPref]] |

### Interactive Appearance Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Standard Background Properties Selector Base | 1325 | Add the selectors below | |
| Black Background Properties Selector Base | 4025 | Add the selectors below | |
| Smart Cursor Selection Box | + 0 | | |
| Smart Cursor Snap Box | + 30 | | |
| Smart Cursor Datum Indicator | + 60 | | |
| Smart Cursor Points | + 90 | | |
| Smart Cursor Edges | + 120 | | |
| Smart Cursor Vector Locks | + 150 | | |
| Smart Cursor Acquisition Hints | + 180 | | |
| Snap Points Available | + 210 | | |
| Current Snap Points | + 240 | | |
| Snap Points Obtained | + 270 | | |
| Snap Points Congestion Indicator | + 300 | | |
| Object Highlighting PreSelection Active Layer | + 330 | | |
| Object Highlighting Selection Active Layer | + 360 | | |
| Object Highlighting Selection Inactive Layer | + 390 | | |
| Object Highlighting Selection Locked | + 420 | | |
| Object Highlighting Snap Object | + 450 | | |
| Object Highlighting Tool Highlighting | + 480 | | |
| Object Highlighting Action | + 510 | | |
| General Exit Edit Context Frame | + 540 | | |
| General Exit Edit Context Show Others | + 570 | | |
| General Page Boundary | + 600 | | |
| General Grid | + 630 | | |
| General Working Plane | + 660 | | |
| General Ground Plane | + 690 | | |
| General Hint Text | + 720 | | |
| General Hint Background | + 750 | | |
| General Reshape Handles Active Layer | + 780 | | |
| General Reshape Handles Inactive Layer | + 810 | | |
| Object Highlighting PreSelection Inactive Layer | + 840 | | |
| Object Highlighting PreSelection Locked | + 870 | | |
| Snap Points Object Oriented | + 900 | | |
| Smart Cursor Planes | + 930 | | |
| Smart Cursor Smart Point Lines | + 960 | | |
| General Repetition Opacity | + 990 | | |
| Smart Cursor Angle Lines | + 1020 | | |
| Object Highlighting Automatic Plane Source | + 1050 | | |
| General XRay Edge Selection | + 1080 | | |
| General Top Plan Backgrond Color | + 1110 | | |
| General Sheet Layer Background Color | + 1140 | | |
| General 3D View Background Color | + 1170 | | |
| General Background Perspective Horizon Sky | + 1200 | | |
| General Background Perspective Horizon Ground | + 1230 | | |
| Object Highlighting Occluded Feedback | + 1260 | | |
| Clip Cube Solid Cut | + 1290 | | |
| Clip Cube Hollow Cut | + 1320 | | |
| Snap Points Master | + 1350 | | |
| Object Highlighting Checked Out | + 1380 | | |
| Subdivision Crease Highlighting | + 1410 | | |
| Ruler Cursor Position Indicators | + 1440 | | |
| Ruler Background | + 1470 | | |
| Ruler Marks and Text | + 1500 | | |
| Floating Databar Background | + 1530 | | |
| Floating Databar Outline and Text | + 1560 | |
| General Object Previews | + 1590 | |
| General Unhide Objects Button | + 1620 | |
| Onscreen View Control Text And Accents | + 1650 | |
| Onscreen View Control Cube | + 1680 | |
| Onscreen View Control Working Plane Cube Face | + 1710 | |
| General Active View Pane Label | + 1740 | |
| Property Available | + 0 | TRUE or FALSE | [VS:GetPref](#) |
| Different Background Color | + 1 | TRUE or FALSE | [VS:GetPref](#) |
| Pattern | + 2 | INTEGER | [VS:GetPrefInt](#) |
| Foreground Color | + 4 | RGB | [VS:GetPrefRGB](#) |
| Background Color | + 5 | RGB | [VS:GetPrefRGB](#) |
| Opacity | + 6 | INTEGER | [VS:GetPrefInt](#) |
| Size | + 7 | REAL | [VS:GetPrefReal](#) |
| Minimum Size | + 8 | REAL | [VS:GetPrefReal](#) |
| Maximum Size | + 9 | REAL | [VS:GetPrefReal](#) |
| Opacity 1 | + 10 | INTEGER | [VS:GetPrefInt](#) |
| Size 1 | + 11 | REAL | [VS:GetPrefReal](#) |
| Minimum Size 1 | + 12 | REAL | [VS:GetPrefReal](#) |
| Maximum Size 1 | + 13 | REAL | [VS:GetPrefReal](#) |
| Opacity 2 | + 14 | INTEGER | [VS:GetPrefInt](#) |

**Example:** To access the Opacity of Object Highlighting Tool Highlighting with a Standard Background use 1811 (1325 + 480 + 6)

## On-Demand Menu Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Use ODM | 6900 | TRUE or FALSE | [VS:GetPref](#) |
| Show ODM After Mouse Idle | 6901 | TRUE or FALSE | [VS:GetPref](#) |
| ODM Mouse Idle Timer | 6902 | INTEGER | [VS:GetPrefInt](#) |
| Show ODM with Spacebar | 6903 | TRUE or FALSE | [VS:GetPref](#) |
| Show ODM with Middle Mouse Button | 6904 | TRUE or FALSE | [VS:GetPref](#) |
| Initialize ODM Layout | 6905 | INTEGER | [VS:GetPrefInt](#) |
| | | 0 (Icon Hint) | [VS:GetPrefInt](#) |
| | | 1 (Text Hint) | [VS:GetPrefInt](#) |
| | | 2 (Icon and Text Hint) | [VS:GetPrefInt](#) |
| | | 3 (Full View) | [VS:GetPrefInt](#) |
| Section ODM Parameters | 6906 | Integer | [VS:GetPrefInt](#) |
| | | 0 (Section ID) | [VS:GetPrefInt](#) |
| | | 1 (Section Type) | [VS:GetPrefInt](#) |
| | | 0 (None) | [VS:GetPrefInt](#) |
| | | 1 (Tool Modes) | [VS:GetPrefInt](#) |
| | | 2 (Snapping Bar) | [VS:GetPrefInt](#) |
| | | 3 (Recent Tools) | [VS:GetPrefInt](#) |
| | | 4 (Standard Views) | [VS:GetPrefInt](#) |
| | | 5 (Tool Sets) | [VS:GetPrefInt](#) |
| | 2 (Quadrant Position) | | |
| | | 0 (Top Left) | [VS:GetPrefInt](#) |
| | | 1 (Top Right) | [VS:GetPrefInt](#) |
| | | 2 (Bottom Left) | [VS:GetPrefInt](#) |
| | | 3 (Bottom Right) | [VS:GetPrefInt](#) |
| | 3 (Tool Set ID) | | |
| Show ODM Search Filters | 7000 | True or False | [VS:GetPref](#) |
| Show ODM Command Context | 7001 | True or False | [VS:GetPref](#) |
| | | 4 (Tool Set Name) |

## Primary Units Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Unit Fraction | 150 | REAL value | [VS:GetPrefReal](#) |
| Units Per Inch | 152 | REAL value | [VS:GetPrefReal](#) |
| Unit Style Name | 153 | STRING value | [VS:GetPrefString](#) |
| Unit Mark | 154 | STRING value | [VS:GetPrefString](#) |
| Sunit Mark | 155 | STRING value | [VS:GetPrefString](#) |
| Sunit Divider | 156 | STRING value | [VS:GetPrefString](#) |
| Smultiplier | 157 | INTEGER value | [VS:GetPrefInt](#) |
| Square Unit Mark | 158 | STRING value | [VS:GetPrefString](#) |
| Square Unit Divisor | 159 | LONGINT | [VS:GetPrefLongInt](#) |
| Cube Unit Mark | 160 | STRING value | [VS:GetPrefString](#) |
| Cube Unit Divisor | 161 | LONGINT | [VS:GetPrefLongInt](#) |
| Display Fraction | 162 | LONGINT value | [VS:GetPrefLongInt](#) |
| Show Unit Mark | 163 | TRUE or FALSE | [VS:GetPref](#) |
| Display Leading Zero | 164 | TRUE or FALSE | [VS:GetPref](#) |
| Display Trailing Zeroes | 165 | TRUE or FALSE | [VS:GetPref](#) |
| Use Minimum Units | 166 | TRUE or FALSE | [VS:GetPref](#) |
| Use Custom Units | 167 | TRUE or FALSE | [VS:GetPref](#) |
| Show Decimals as Fractions | 168 | TRUE or FALSE | [VS:GetPref](#) |
| Dimension Precision | 169 | LONGINT value | [VS:GetPrefLongInt](#) |
| Predefined Units Style | 170 | 1 (Feet & Inches) | [VS:GetPrefInt](#) |
| | | 2 (Inches) | [VS:GetPrefInt](#) |
| | | 3 (Feet) | [VS:GetPrefInt](#) |
| | | 4 (Yards) | [VS:GetPrefInt](#) |
| | | 5 (Miles) | [VS:GetPrefInt](#) |
| | | 6 (Microns) | [VS:GetPrefInt](#) |
| | | 7 (Millimeters) | [VS:GetPrefInt](#) |
| | | 8 (Centimeters) | [VS:GetPrefInt](#) |
| | | 9 (Meters) | [VS:GetPrefInt](#) |
| | | 10 (Kilometers) | [VS:GetPrefInt](#) |
| | | 11 (Degrees – Landmark & Azimuth only) | [VS:GetPrefInt](#) |
| Fractional Display Precision | 171 | LONGINT value | [VS:GetPrefLongInt](#) |
| Fractional Dimension Precision | 172 | LONGINT value | [VS:GetPrefLongInt](#) |
| Metric Unit Flag | 173 | TRUE or FALSE | [VS:GetPref](#) |
| Angular Unit | 174 | 0 (degrees) | [VS:GetPrefInt](#) |
| | | 1 (radians) | [VS:GetPrefInt](#) |
| | | 2 (gradians) | [VS:GetPrefInt](#) |
| Round Fraction to Decimal | 175 | TRUE or FALSE | [VS:GetPref](#) |
| Area Units Per Square Inch | 176 | REAL value | [VS:GetPrefReal](#) |
| Area Unit Name | 177 | STRING value | [VS:GetPrefString](#) |
| Area Unit Mark | 178 | STRING value | [VS:GetPrefString](#) |
| Area Precision | 179 | LONGINT value | [VS:GetPrefLongInt](#) |
| Volume Units Per Cubic Inch | 180 | REAL value | [VS:GetPrefReal](#) |
| Volume Unit Name | 181 | STRING value | [VS:GetPrefString](#) |
| Volume Unit Mark | 182 | STRING value | [VS:GetPrefString](#) |
| Volume Precision | 183 | LONGINT value | [VS:GetPrefLongInt](#) |
| Use Custom Area Units | 184 | TRUE or FALSE | [VS:GetPref](#) |
| Use Custom Volume Units | 185 | TRUE or FALSE | [VS:GetPref](#) |
| Area Unit Fraction | 186 | REAL value | [VS:GetPrefReal](#) |
| Volume Unit Fraction | 187 | REAL value | [VS:GetPrefReal](#) |
| Display Rounding Base | 188 | 0 (1) | [VS:GetPrefInt](#) |
| | | 1 (2.5) | [VS:GetPrefInt](#) |
| | | 2 (5) | [VS:GetPrefInt](#) |
| Dimension Rounding Base | 189 | 0 (1) | [VS:GetPrefInt](#) |
| | | 1 (2.5) | [VS:GetPrefInt](#) |
| | | 2 (5) | [VS:GetPrefInt](#) |
| Dimension Rounding Base | 190 | 0 (regular style) | [VS:GetPrefInt](#) |
| | | 1 (diagonal style) | [VS:GetPrefInt](#) |
| | | 2 (horizontal style) | [VS:GetPrefInt](#) |
| Show Thousands Separator | 191 | TRUE or FALSE | [VS:GetPref](#) |
| Save and Restore Unit1 | 192 | TRUE or FALSE | [VS:GetPref](#) |
| HiddenLineDashType | 197 | Integer value | [VS:GetPrefInt](#) |
| Default Dimension Class ID | 546 | RefNumber | [VS:GetPrefLongInt](#) |

### Secondary Units Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Unit Fraction | 200 | REAL value | [VS:GetPrefReal](VS:GetPrefReal) |
| Units Per Inch | 202 | REAL value | [VS:GetPrefReal](VS:GetPrefReal) |
| Unit Style Name | 203 | 64 character STRING | [VS:GetPrefString](VS:GetPrefString) |
| Unit Mark | 204 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| Sunit Mark | 205 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| Sunit Divider | 206 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| Smultiplier | 207 | INTEGER value | [VS:GetPrefInt](VS:GetPrefInt) |
| Square Unit Mark | 208 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| Square Unit Divisor | 209 | LONGINT | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Cube Unit Mark | 210 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| Cube Unit Divisor | 211 | LONGINT value | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Display Fraction | 212 | LONGINT value | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Show Unit Mark | 213 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Display Leading Zero | 214 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Display Trailing Zeroes | 215 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Use Minimum Units | 216 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Use Custom Units | 217 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Show Decimals as Fractions | 218 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Dimension Precision | 219 | LONGINT value | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Predefined Units Style | 220 | 1 (Feet & Inches) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 2 (Inches) | " |
|  |  | 3 (Feet) | " |
|  |  | 4 (Yards) | " |
|  |  | 5 (Miles) | " |
|  |  | 6 (Microns) | " |
|  |  | 7 (Millimeters) | " |
|  |  | 8 (Centimeters) | " |
|  |  | 9 (Meters) | " |
|  |  | 10 (Kilometers) | " |
|  |  | 11 (Degrees – Landmark & Azimuth only) | " |
| Fractional Display Precision | 221 | LONGINT value | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Fractional Dimension Precision | 222 | LONGINT value | [VS:GetPrefLongInt](VS:GetPrefLongInt) |
| Metric Unit Flag | 223 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Angular Unit | 224 | 0 (degrees) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 1 (radians) | " |
|  |  | 2 (gradians) | " |
| Round Fraction to Decimal | 225 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Dimension Rounding Base | 226 | 0 (1) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 1 (2.5) | " |
|  |  | 2 (5) | " |

### DXF Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Auto Units | 300 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Units | 301 | INTEGER | [VS:GetPrefInt](VS:GetPrefInt) |
| DXF Units Per Inch | 302 | REAL | [VS:GetPrefReal](VS:GetPrefReal) |
| Auto Model Space Scale | 303 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Model Space Scale | 304 | REAL | [VS:GetPrefReal](VS:GetPrefReal) |
| 2D 3D Import Handling | 305 | INTEGER | [VS:GetPrefInt](VS:GetPrefInt) |
| Map Layers to Classes | 306 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Convert Mlines to Walls | 307 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Convert Rays and Xlines | 308 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Scale Dash Lengths | 309 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Dash Length Scale | 310 | REAL | [VS:GetPrefReal](VS:GetPrefReal) |
| Auto Block Attribute Handling | 311 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Block Attribute Handling | 312 | INTEGER | [VS:GetPrefInt](VS:GetPrefInt) |
| Auto Point Handling | 313 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Convert Points to Loci | 314 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Point Symbols are Guides | 315 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Map Colors to Line Weights | 316 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Set Line Colors Black | 317 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Paper Space Units | 318 | INTEGER | [VS:GetPrefInt](VS:GetPrefInt) |
| Auto Scale Dash Lengths | 319 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Group Record Fields | 320 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Auto Line Weight Handling | 321 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Convert Dimensions To Groups | 322 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Rays and Lines To Guides | 323 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Auto Center After Import | 324 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Center After Import | 325 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Use World Origin | 326 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Set Vectorworks Units To Match | 327 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Add Prefix To DXF Layers | 328 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Prefix To DXF Edit | 329 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| External Refs Handling | 330 | 0 (bind external refs) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 1 (ignore external refs) | " |
|  |  | 2 (create VW refs) | " |
|  |  | 3 (use layer import) | " |
| ADT Objects 2D View | 331 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Ignore Block Clipping | 334 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Conversion Ref | 335 | 0 (VW Conversion Res) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 1 (Low) |  |
|  |  | 2 (Medium) |  |
|  |  | 3 (High) |  |
|  |  | 4 (Very High) |  |
| Convert Tables To Worksheets | 338 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Import As Solid Line | 339 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Smallest Gap | 340 | REAL | [VS:GetPrefReal](VS:GetPrefReal) |
| Import Textures | 341 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Purge Unused Blocks | 344 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Purge Unused Layers | 345 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Purge Unused Dim Styles | 346 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Purge Unused Line Types | 347 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| Purge Unused Materials | 348 | TRUE or FALSE | [VS:GetPref](VS:GetPref) |
| CL Mapping Name | 349 | STRING value | [VS:GetPrefString](VS:GetPrefString) |
| GeoRef Import Type | 350 | 0 (None) | [VS:GetPrefInt](VS:GetPrefInt) |
|  |  | 1 (UseDocument) |  |
|  |  | 2 (User) |  |
|  |  | 3 (UserAndAplly) |  |
| GeoRef Import Type | 351 | STRING value | [VS:GetPrefString](VS:GetPrefString) |

## Structural Units

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Mass Units | 6821 | INTEGER | [VS:GetPrefInt](#) |
| | | 0 (Milligram) | |
| | | 1 (Gram) | |
| | | 2 (Kilogram) | |
| | | 3 (Tonne) | |
| | | 4 (Ounce) | |
| | | 5 (Pound) | |
| | | 6 (Stone) | |
| | | 7 (Quarter) | |
| | | 8 (Hundred Weight UK) | |
| | | 9 (Hundred Weight US) | |
| | | 10 (Short Ton) | |
| | | 11 (Long Ton) | |
| | | 12 (Custom) | |
| Mass Unit Precision | 6822 | INTEGER | [VS:GetPrefInt](#) |
| Show Unit Mark | 6823 | TRUE or FALSE | [VS:GetPref](#) |
| Current Unit Mark | 6824 | STRING (Read Only) | [VS:GetPrefString](#) |
| Unit Name | 6825 | STRING (Read Only) | [VS:GetPrefString](#) |
| Mass Unit Scale per Gram | 6826 | Real (Read Only) | [VS:GetPrefReal](#) |
| Force Unit Index | 6827 | Integer | [VS:GetPrefInt](#) |
| | | 0 (Newton) | |
| | | 1 (Kilonewton) | |
| | | 2 (Ounce Force) | |
| | | 3 (Pound Force) | |
| | | 4 (Custom) | |
| Force Unit Precision | 6828 | Integer | [VS:GetPrefInt](#) |
| Show Force Unit Mark | 6829 | TRUE or FALSE | [VS:GetPref](#) |
| Force Unit Mark | 6830 | STRING (Read Only) | [VS:GetPrefString](#) |
| Force Unit Name | 6831 | STRING (Read Only) | [VS:GetPrefString](#) |
| Force Unit Scale per Neuton | 6832 | REAL (Read Only) | [VS:GetPrefReal](#) |
| Distributed Mass Unit Index | 6833 | INTEGER | [VS:GetPrefInt](#) |
| | | 0 (Gram per Millimeter) | |
| | | 1 (Kilogram per Meter) | |
| | | 2 (Ounce per Inch) | |
| | | 3 (Pound per Foot) | |
| | | 4 (Custom) | |
| Distributed Mass Unit Precision | 6834 | INTEGER | [VS:GetPrefInt](#) |
| Distributed Mass Unit Show Unit Mark | 6835 | TRUE or FALSE | [VS:GetPref](#) |
| Distributed Mass Unit Mark | 6836 | STRING | [VS:GetPrefString](#) |
| Distributed Mass Unit Name | 6837 | STRING (Read Only) | [VS:GetPrefString](#) |
| DistributedMassUnit Scale Grams per Millimeter | 6838 | REAL (Read Only) | [VS:GetPrefReal](#) |

## Gradient and Image Fill Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| Default Gradient Fill | 508 | LONGINT | [VS:GetPrefLongInt](#) |
| Default Gradient Fill Angle | 512 | REAL | [VS:GetPrefReal](#) |
| Default Gradient Fill Repeat | 513 | TRUE or FALSE | [VS:GetPref](#) |
| Default Gradient Fill Geometric Type | 515 | INTEGER | [VS:GetPrefInt](#) |
| Default Gradient Fill Mirror | 516 | TRUE or FALSE | [VS:GetPref](#) |
| Default Image Fill Maintain Aspect Ratio | 517 | TRUE or FALSE | [VS:GetPref](#) |
| Default Image Fill | 518 | LONGINT | [VS:GetPrefLongInt](#) |
| Default Image Fill Angle | 523 | REAL | [VS:GetPrefReal](#) |
| Default Image Fill Repeat | 524 | TRUE or FALSE | [VS:GetPref](#) |
| Default Image Fill Mirror | 526 | TRUE or FALSE | [VS:GetPref](#) |
| Default Image Fill Flip | 527 | TRUE or FALSE | [VS:GetPref](#) |
| Default Image Fill I-Length | 532 | REAL (current units) | [VS:GetPrefReal](#) |
| Default Image Fill J-Length | 533 | REAL (current units) | [VS:GetPrefReal](#) |
| Default Fill Style | 528 | LONGINT | [VS:GetPrefLongInt](#) |
| Default Fill Type | 529 | INTEGER | [VS:GetPrefInt](#) |
| Default Hatch Fill | 530 | LONGINT | [VS:GetPrefLongInt](#) |

## Misc. Preference Selectors

| Preference | Selector | Preference Data Type | Function |
|------------|----------|----------------------|----------|
| RenderWorks Enabled | 240 | TRUE or FALSE | [VS:GetPref](#) |
| Disable RenderWorks | 241 | TRUE or FALSE | [VS:GetPref](#) |
| PDF Page Object Paint Node Resolution | 270 | LONGINT (DPI) | [VS:GetPrefLongInt](#) |
| Don't Cache Plug-in Scripts | 407 | TRUE or FALSE | [VS:GetPref](#) |
| Auto Refresh Mode | 450 | TRUE or FALSE | [VS:GetPref](#) |
| Window Zoom Factor | 500 | REAL | [VS:GetPrefReal](#) |
| Layer Options | 506 | INTEGER | [VS:GetPrefInt](#) |
| Class Options | 507 | INTEGER | [VS:GetPrefInt](#) |
| Hide Wall Cavity Threshold | 540 | INTEGER | [VS:GetPrefInt](#) |
| Save Viewport Cache | 541 | TRUE or FALSE | [VS:GetPref](#) |
| Smooth Mesh | 542 | TRUE or FALSE | [VS:GetPref](#) |
| Mesh Crease Angle | 543 | REAL | [VS:GetPrefReal](#) |
| Use Auto Draw Coord | 544 | TRUE or FALSE | [VS:GetPref](#) |
| Show Text Files in Plugin Editor | 560 | TRUE or FALSE | [VS:GetPref](#) |
| Release Version Integer | 570 | INTEGER | [VS:GetPrefInt](#) |
| Symbol Tool Insert Mode | 580 | INTEGER | [VS:GetPrefInt](#) |
| Symbol Tool Wall Insertion | 581 | TRUE or FALSE | [VS:GetPref](#) |
| Symbol Tool Alignement Mode | 582 | INTEGER | [VS:GetPrefInt](#) |
| Parametric Enable State Eventing | 590 | INTEGER | [VS:GetPrefInt](#) |
| Update Text Style Size | 685 | TRUE or FALSE | [VS:GetPref](#) |
| Hide Non Detail | 705 | TRUE or FALSE | [VS:GetPref](#) |
| DVLP Position Locked | 709 | TRUE or FALSE (Read Only) | [VS:GetPref](#) |
| Display Horizontal DPI | 1011 | REAL (read-only) | [VS:GetPrefReal](#) |
| Display Vertical DPI | 1012 | REAL (read-only) | [VS:GetPrefReal](#) |
| Screen Plane Mode | 1099 | TRUE or FALSE | [VS:GetPref](#) |
| Windows 64bit OS | 1100 | TRUE or FALSE (read-only) | [VS:GetPref](#) |
| Is Autoplane Active | 1101 | TRUE or FALSE | [VS:GetPref](#) |
| Plane Mode is set to ScreenOrWorkingPlane | 1102 | TRUE or FALSE (read-only) | [VS:GetPref](#) |
| Enable online content | 1104 | TRUE or FALSE | [VS:GetPref](#) |
| Enable Subscription Libraries | 1106 | TRUE or FALSE | [VS:GetPref](#) |
| Use Same Visibilities in All Panes | 1107 | TRUE or FALSE | [VS:GetPref](#) |
| GeoRef Layer | 1117 | INTEGER | [VS:GetPrefInt](#) |
| Compact Document Planes | 565 | TRUE or FALSE (write-only) | [VS:GetPref](#) |
| Number of Document Planes | 566 | LONGINT | [VS:GetPrefLongInt](#) |
| Max Document Planes | 567 | LONGINT | [VS:GetPrefLongInt](#) |
| Plan Rotation Paused | 591 | TRUE or FALSE (read-only) | [VS:GetPref](#) |
| Plan Rotation Paused Angle | 592 | REAL (read-only) | [VS:GetPrefReal](#) |
| Use Screen and Working Plane | 1102 | TRUE or FALSE | [VS:GetPref](#) |
| Perspective Cropped | 127 | TRUE or FALSE | [VS:GetPref](#) |
| Use Old 2D Pan and Zoom | 128 | TRUE or FALSE | [VS:GetPref](#) |
| Interactive Zoom Pan Mode | 6704 | TRUE or FALSE | [VS:GetPref](#) |
| Heliodon Interactive Render | 6706 | TRUE or FALSE | [VS:GetPref](#) |
| Show Clip Cube | 6707 | TRUE or FALSE | [VS:GetPref](#) |
| Write VS Binary Mode | 6708 | TRUE or FALSE | [VS:GetPref](#) |
| Show Hidden Line Surface Hatches | 280 | TRUE or FALSE | [VS:GetPref](#) |
| Show Hidden Line Text And Markers | 281 | TRUE or FALSE | [VS:GetPref](#) |
| Show Linear Direction Marker | 6719 | TRUE or FALSE | [VS:GetPref](#) |
| Feedback Scale Factor | 6716 | REAL (read-only) | [VS:GetPrefReal](#) |
| Feedback Resolution | 6717 | REAL (read-only) | [VS:GetPrefReal](#) |
| Document Window Resolution | 671 | REAL (read-only) | [VS:GetPrefReal](#) |
| Show Internal Origin Marker | 6723 | TRUE or FALSE | [VS:GetPref](#) |
| Always Show Current Tool On FDB | 9999 | TRUE or FALSE | [VS:GetPref](#) |
| Display Hidden Objects Ghosted | 604 | TRUE or FALSE | [VS:GetPref](#) |
| Low Detail Exist Comp Objs | 605 | TRUE or FALSE | [VS:GetPref](#) |
| Low Detail Exist SymsPios | 606 | TRUE or FALSE | [VS:GetPref](#) |
| Low Detail Removed Comp Objs | 607 | TRUE or FALSE | [VS:GetPref](#) |
| Low Detail Removed SymsPios | 608 | TRUE or FALSE | [VS:GetPref](#) |
| Alt Attrib Removed Objs | 609 | TRUE or FALSE | [VS:GetPref](#) |
| CurrentLayerScale | 6757 | Real (read-only) | [VS:GetPrefReal](#) |
| Save VGM Cache | 6840 | TRUE or FALSE | [VS:GetPref](#) |

### Notes:
#### Symbol Tool Insert Mode:
- 1 - Regular Insertion
- 2 - Offset Insertion
- 3 - Pick-up Mode

#### Symbol Tool Alignement Mode:
- 1 - Left
- 2 - Center
- 3 - Right
- 4 - Natural
