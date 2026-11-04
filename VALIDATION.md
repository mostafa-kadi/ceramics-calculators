# Scientific validation notes

## Independent numerical reference checks

| Calculator | Reference inputs | Expected result |
|---|---|---:|
| Theoretical density | M = 233.19 g mol⁻¹; Z = 1; V = 64 Å³ | 6.050330 g cm⁻³ |
| Bulk density | m = 5 g; V = 1.25 cm³ | 4.000000 g cm⁻³ |
| Relative density | ρbulk = 5; ρtheory = 5.5 g cm⁻³ | 90.909091% |
| Porosity estimate | ρbulk = 5; ρtheory = 5.5 g cm⁻³ | 9.090909% |
| Archimedes density | Wdry = 4.8 g; Wsat = 5 g; Wsusp = 3 g; ρliquid = 0.997 g cm⁻³ | 2.392800 g cm⁻³ |
| Linear shrinkage | L0 = 20 mm; Lf = 18.5 mm | 7.500000% |
| Volumetric shrinkage (isotropic estimate) | L0 = 20 mm; Lf = 18.5 mm | 20.854688% |

## Scope and assumptions

- Theoretical density uses ρ = ZM/(NA Vcell), with Vcell converted from Å³ to cm³. Z and M must refer to the same crystallographic formula-unit definition.
- Bulk density uses the externally measured specimen volume.
- Relative density and porosity assume the supplied theoretical density is the pore-free reference density for the actual phase assemblage and composition.
- Porosity is estimated as 1 − ρbulk/ρtheory; this does not distinguish open from closed porosity.
- Archimedes density assumes adequate liquid infiltration/saturation, no trapped bubbles, correct removal of surface liquid, and liquid density at the measurement temperature. The current tool calculates bulk density from the supplied dry, saturated and suspended masses.
- Shrinkage is linear shrinkage along the measured direction, not volumetric shrinkage.

## Validation status

The example outputs were independently recalculated from the equations and match the application's numerical outputs. Invalid zero/negative mass or volume and inconsistent Archimedes mass ordering are rejected.

This does not replace measurement uncertainty analysis, phase-purity assessment, or a laboratory SOP for Archimedes measurements.