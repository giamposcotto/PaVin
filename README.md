# Anchored Sheet Pile Wall Embedment & Analysis Tool

A Python-based geotechnical engineering application for Windows designed to compute the strictly necessary embedment depth and generate interaction diagrams for top-restrained (anchored) sheet pile walls.

---

## 📌 Repository Description (For GitHub Setup)

> **Short Description / Tagline:**
> *A Python desktop app for Windows to calculate the minimum required embedment depth and interaction diagrams for top-restrained sheet pile walls.*

---

## 🚀 Key Features

* **Embedment Depth Calculation:** Computes the exact required depth of embedment ($d$) for single-propped/anchored sheet pile walls using limit equilibrium principles.
* **Restraint Placement:** Flexible positioning of the top restraint (anchor line or tie-back prop) relative to the top of the wall.
* **Soil & Hydraulic Parameters:**
  * Active ($K_a$) and passive ($K_p$) earth pressure coefficients.
  * Soil mechanical properties (unit weight $\gamma$, internal friction angle $\phi'$).
  * Hydraulic permeability parameters ($k$) for seepage and effective stress analysis.
* **Structural Interaction Plots:** Generates bending moment and shear force diagrams along the entire length of the sheet pile wall.
* **Built-in Examples:** Includes two pre-loaded sample configuration files directly accessible within the interface.
* **Standalone Windows Executable:** Entirely written in Python and compiled for seamless deployment on Windows OS.

---

## ⚙️ Technical Methodology

### 1. Anchored Wall Limit Equilibrium (Free Earth Support Method)
Unlike cantilever walls, top-restrained sheet pile walls benefit from a propped boundary condition near the top. Static equilibrium balances soil thrusts, anchor force ($T$), and passive soil resistance.

By taking moments about the point of restraint ($z = z_a$):

$$\sum M_{anchor} = 0 \implies \int_{z_a}^{H+d} \sigma_n(z) \cdot (z - z_a) \, dz = 0$$

where:
* $H$: Retention height of the backfill
* $d$: Depth of embedment below the excavation line
* $z_a$: Depth of the top restraint
* $\sigma_n(z)$: Net lateral pressure ($\sigma_a - \sigma_p + u$)

### 2. Anchor Force & Section Forces
Once the embedment depth $d$ is determined, horizontal equilibrium ($\sum F_x = 0$) yields the anchor tension $T$, allowing the full shear force $V(z)$ and bending moment $M(z)$ diagrams to be plotted across the wall profile.

---

## 💡 Quick Start

1. **Launch App:** Run the application on any Windows machine.
2. **Load Integrated Examples:** Open one of the two integrated example files from the menu.
3. **Define Retention & Restraint:** Enter retaining height $H$ and top restraint level $z_a$.
4. **Input Soil Parameters:** Set soil weight, active ($K_a$) / passive ($K_p$) coefficients, and permeability values.
5. **Calculate & View Diagrams:** Compute required depth $d$, anchor force $T$, and view interactive internal force diagrams.

---

## 🏷️ Suggested GitHub Topics

`geotechnical-engineering` `sheet-pile-wall` `anchored-wall` `embedment-depth` `earth-pressure` `retaining-structure` `python-gui` `windows-app` `civil-engineering`
