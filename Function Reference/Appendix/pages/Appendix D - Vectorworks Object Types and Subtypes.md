# Appendix D - Vectorworks Object Types and Subtypes

The numeric types in the table below are useful for identifying what type of object is referenced by a handle. The function [VS:GetTypeN](h) will return one of these numeric types. The Criteria values in the table below are used in search criteria statements. They are used along with the criteria *T=* to search for objects of a specific type. For example, the following statement will count the number of rectangles in the active document:

```python
Message( Count(T=RECT) );
```

## Object Types

| Object | Type | Criteria |
|--------|------|----------|
| Line | 2 | LINE |
| Rectangle | 3 | RECT |
| Oval | 4 | OVAL |
| Polygon | 5 | POLY |
| Arc | 6 | ARC |
| Freehand | 8 | FHAND |
| 3D Locus | 9 | LOCUS3D |
| Text | 10 | TEXT |
| Group | 11 | GROUP |
| Rounded rectangle | 13 | RRECT |
| Bitmap Image | 14 | BITMAP |
| Symbol instance | 15 | SYMBOL |
| Symbol Definition (1) | 16 |  |
| 2D Locus | 17 | LOCUS |
| Worksheet (1) | 18 | SPRDSHEET |
| Material definition (1) | 19 | MATERIAL |
| Polyline | 21 | POLYLINE |
| PICT Image | 22 | PICT |
| Extrude | 24 | XTRD |
| 3D Polygon | 25 | POLY3D |
| Layer Link | 29 | LAYERLINK |
| Layer | 31 |  |
| Sweep | 34 | SWEEP |
| Multiple extrude | 38 | MXTRD |
| Mesh | 40 | MESH |
| Mesh vertex | 41 |  |
| Record Definition (Format) | 47 |  |
| Record | 48 |  |
| Document script (1) | 49 |  |
| Script palette (1) | 51 |  |
| Worksheet Data (on drawing) | 56 |  |
| Dimension | 63 | DIMENSION |
| Hatch Fill definition (1) | 66 |  |
| Wall | 68 | WALL |
| Column, Floor, Roof Face | 71 | SLAB |
| Light | 81 | LIGHT |
| Roof edge | 82 |  |
| Roof object | 83 | ROOF |
| CSG Solid (Addition, Subtraction) | 84 | CSGSOLID |
| Plug-in object | 86 | PLUGINOBJECT |
| Roof element | 87 | ROOFELEMENT |
| Symbol folder (1) | 92 |  |
| Texture Bitmap (1) | 93 |  |
| Class Definition (1) | 94 |  |
| Solid (Cone, Sphere, ...) | 95 | SOLID |
| Line Type definition (1) | 96 |  |
| Texture definition (1) | 97 |  |
| Roof Style definition (1) | 102 |  |
| Slab Style definition (1) | 107 |  |
| Tile Fill definition (1) | 108 |  |
| Text Style definition (1) | 109 |  |
| NURBS Curve | 111 | NURBSCURVE |
| NURBS Surface | 113 | NURBSSURFACE |
| Renderworks Background (1) | 115 |  |
| Image Fill definition (1) | 119 |  |
| Gradient Fill definition (1) | 120 |  |
| Fill Space (1) | 121 |  |
| Viewport | 122 | VIEWPORT |
| Wall Style definition (1) | 127 |  |

**Notes:**
1. These special objects are not directly displayed in the document. They may contain definition information used by other objects or features.

## Object Subtypes

| Object | Type | Criteria |
|--------|------|----------|
| Directional Light | 500 | DIRLIGHT |
| Spot Light | 501 | SPOTLIGHT |
| Point Light | 502 | POINTLIGHT |
| Custom Light | 503 | CUSTLIGHT |
| Area Light | 504 | AREALIGHT |
| Line Light | 505 | LINELIGHT |
| Sheet Layer Viewport | 506 | REGVIEWPORT |
| Section Viewport | 507 | SECTVIEWPORT |
| Floor | 508 | FLOOR |
| Roof Face | 509 | ROOFFACE |
| Pillar | 510 | PILLAR |
| Cone | 511 | CONE |
| Sphere | 512 | SPHERE |
| Hemisphere | 513 | HEMISPHERE |
| Circle | 514 | CIRCLE |
| Opened Arc | 515 | OPENEDARC |
| Solid Subtraction | 516 | CSGSUBTR |
| Solid Addition | 517 | CSGADD |
| Solid Intersection | 518 | CSGINTER |
| Solid Section | 519 | CSGSECT |
| Solid Shell | 520 | CSGSHELL |
| Chamfer | 521 | CSGCHAMFER |
| Fillet | 522 | CSGFILLET |
| Control point based NURBS surface | 523 | NURBSSURFCTRLP |
| Interpolated NURBS surface | 524 | NURBSSURFINTERP |

**Notes:**
1. These special objects are not directly displayed in the document. They may contain definition information used by other objects or features.
