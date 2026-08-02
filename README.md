# Four-Legged Robot

A four-legged walking robot designed in SolidWorks, with fully articulated legs — each
leg moves as a linkage rather than being a fixed part. This repo holds the CAD, an
interactive 3D preview, and neutral export formats that open without SolidWorks.

## 3D preview

**[▶ Open the interactive 3D model](finalbotview.STL)** — click to rotate, pan, and zoom
right here on GitHub.
![Preview](preview.png)

## Design

- **Layout:** central chassis (top and bottom body plates, side and front fenders,
  component mounts) with four articulated legs.
- **Legs:** each leg is a multi-segment movable linkage built from a common set of parts
  (`botrightleg1` through `botrightleg7` plus pivots), so all four legs share the same
  mechanism and can move.
- **Material:** plain carbon steel (E ≈ 200 GPa, ρ ≈ 7850 kg/m³) in the current model.

<!-- Optional, if you want to add it:
- Gait / how the legs actuate (degrees of freedom per leg, drive method)
- Intended build: 3D printed / machined, target size
- What drove the design (class project / personal build)
-->

## A note on material and mass

The model is currently plain carbon steel, which is dense. At real scale the assembly
comes out heavy for legs this slender. For an actual build, a lighter material (aluminum
or a printed polymer) would cut the mass dramatically while keeping the geometry; steel is
fine as the baseline CAD material but isn't the practical build choice.

## Files

- `cad/` — SolidWorks parts (`.SLDPRT`) and assemblies (`.SLDASM`)
- `four-leg-bot.stl` — mesh export for the 3D preview / printing
- `four-leg-bot.step` — neutral CAD format (opens in any CAD tool)

## Notes

Native SolidWorks files are stored via Git LFS. To open the full parametric model you'll
need SolidWorks; for viewing or printing, use the STL or STEP.
