# Cologne Cathedral (Kölner Dom) — Parametric 4-Color 3D Model & Interactive Viewer

## 1. Architectural Features Preserved

Generated procedurally from `source/rebuild.py` at **1:1000 scale**
(`164.0 × 104.0 × 163.4 mm` including the `6.0 mm` stepped plinth base;
spire height `157.4 mm` above base):

- **Twin Towers (`Westbau`)**: Four distinct Gothic architectural stories
  per tower with stepped corner buttresses, belfry lancets, freestanding
  corner pinnacles, and octagonal upper drums.
- **Openwork Filigree Spires**: Eight inclined crocketed corner ribs
  converging to the finial (`Kreuzblume`), stiffened by seven horizontal
  octagonal tracery rings.
- **Gothic Portals (5)**: Deeply recessed West Central Portal (`Petersportal`),
  flanking North/South West portals, and North/South Transept triple-portals
  with pointed archivolts and wimberg gables.
- **Rose Windows (3) & Clerestory Lancets**: Great West Facade 12-spoke
  wheel rose window and North/South Transept rose windows over stained-glass
  discs.
- **Double-Tier Flying Buttresses (26 Assemblies)**: Intermediate and outer
  buttress piers crowned with crocketed pinnacles (`Fialen`) and double-tier
  inclined flying arches along the Nave, Choir, and East Chevet.
- **Radiating Apse (`Chorkapellen`)**: Seven polygonal radiating chapels
  surrounding the East ambulatory and high choir apse.
- **Four-Color AMS Material Partitioning**:
  1. `Slot 1 (stone_main / #D8C8B0)`: Warm Rhenish sandstone walls, towers,
     piers, and terrace.
  2. `Slot 2 (stone_dark / #6E655C)`: Weathered dark basalt openwork spires,
     pinnacles, crockets, flying buttress coping caps, and lower plinth.
  3. `Slot 3 (roof_patina / #4A7C6B)`: Patinated verdigris copper roofs and
     central crossing flèche (`Dachreiter`).
  4. `Slot 4 (stained_glass / #2B5B84)`: Rose windows and pointed Gothic
     lancet windows.

## 2. Actual Validation Results (`source/rebuild.py`)

| Metric | Actual Result | Status |
| :--- | :--- | :--- |
| **Bounding Box (X × Y × Z)** | `164.0 × 163.4 × 104.0 mm` | **PASSED** |
| **Watertight Manifold Check** | `100% Closed Manifold Solids` | **PASSED** |
| **Positive Signed Volume** | `100% Positive Orientation` | **PASSED** |
| **Minimum Rib / Feature Wall** | `0.88 mm` (≥ `0.80 mm` threshold for 0.4 mm nozzle) | **PASSED** |
| **Physical 3D Printing** | Not physically printed | **UNVERIFIED** |
| **Physical Assembly Fit** | Not physically assembled | **UNVERIFIED** |

## 3. Recommended Print Settings

- **Nozzle**: 0.4 mm
- **Layer height**: 0.12–0.16 mm
- **Supports**: Recommended for openwork spires and flying arches
- **Scale**: 1:1000 → footprint 164 × 104 mm, height 163.4 mm
- **Filaments (4 slots)**:
  1. Rhenish Sandstone → `#D8C8B0`
  2. Weathered Basalt → `#6E655C`
  3. Patinated Copper → `#4A7C6B`
  4. Gothic Stained Glass → `#2B5B84`

## 4. Verification Disclosure

Digital parametric geometry, 4-color material partitioning, bounding-box
dimensions, and manifold checks have been programmatically verified via
`source/rebuild.py`. **Physical 3D printing and physical assembly remain
UNVERIFIED** as no physical print run has been executed.