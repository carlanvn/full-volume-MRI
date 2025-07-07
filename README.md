# full-volume-MRI

This repository provides **sample full volume magnetic resonance imaging (MRI) datasets** of **displacements** and **Lagrangian strains** for **intact and torn ovine rotator cuff tendons**, viewable in [ParaView](https://www.paraview.org/).

## 📁 Folder Structure

The repository includes two folders:
- `20231012/`
- `20231107/`

Each folder corresponds to the **timestamp of the experiment** and contains both **displacement** and **strain** datasets.

## 📈 Displacement Data

Displacement fields are available for both **intact** and **torn** meshes.

- File prefixes indicate the **phase unwrapping method** used:
  - `Jon`: Code developed by Professor Jon Estrada
  - `sunwrap`: MATLAB function available publicly

## 💠 Strain Data

Strain datasets are provided for the **torn mesh**, including:
- `LagrangeNormal`: Normal strain components of the Lagrangian strain tensor (E₁₁, E₂₂, E₃₃)
- `LagrangeShear`: Shear strain components of the Lagrangian strain tensor (E₁₂, E₁₃, E₂₃)
- `maxShear`: Maximum shear strain

## 🧩 File Naming Convention for Strain Files

Strain filenames follow the format:

TIMESTAMPStrainType_XY.xdmf

Where:
- `X` = Type of strain component (normal or shear)
  - `1` = 1 mm
  - `2` = 2 mm
- `Y` = Condition  
  - `1` = Intact
  - `2` = Torn

The first index represents the amount of experimental elongation. The second index represent the condition of the tendon.

### Example:
- `20231107LagrangeNormal_12.xdmf` contains **normal strain** components for a **1 mm stretch in the torn condition**.

---

## 📚 How to Cite

If you use these datasets, please cite the following preprint:

> Villacís Núñez, C. N., Scheven, U., Bedi, A., Arruda, E. M. (2025). *Tear Growth Mechanisms in High-Grade Bursal-Sided Partial Thickness Tears in the Rotator Cuff Measured with Full Volume Methods*. Preprint: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5202182

This citation will be updated upon publication in a peer-reviewed journal.

---
