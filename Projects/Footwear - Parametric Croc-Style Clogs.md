---
title: "Project: Parametric Croc-Style Clogs"
created: 2026-09-05
tags:
  - 3d-printing
  - project
  - footwear
  - clogs
  - tpu
status: Ready to Slice # [Idea, Ready to Slice, In Progress, Completed]
material_main: Bambu TPU 95A (or Foaming TPU)
material_aux: None
nozzle_size: 0.4mm Hardened Steel
print_time: ~14h – 18h per shoe
filament_used_grams: ~320g – 420g per shoe
---

# 🩴 Project: Parametric Croc-Style Clogs

A fully 3D-printed, single-piece ergonomic clog featuring ventilation ports, a cupped heel bed, and a shock-absorbing Gyroid cushioned sole.

---

## 📌 Project Overview
* **Model Inspiration / Source:**
  * [MakerWorld: Crocs Shoes - Fully 3D-printed (MakerVerse Designs)](https://makerworld.com/en/search/models?keyword=crocs+shoes)
  * [Printables: Parametric Clogs & Slip-On Slides](https://printables.com/search/models?q=tpu+clogs)
* **Design Type:** 1-piece monocoque print (sole, upper, and heel strap all printed in a single run).
* **Target Filament:** **TPU 95A** (durable, high grip) or **ColorFabb varioShore Foaming TPU** (cloud-soft lightweight finish).

---

## 📏 Sizing & Scaling Chart

To get a custom fit, measure your foot length in millimeters with athletic socks on, then apply the scale factor in Bambu Studio:

| US Men's Size | US Women's Size | EU Size | Foot Length ($L_{\text{foot}}$) | Target Internal Length | Recommended Scale % |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **US 7** | US 8.5 | EU 40 | 250 mm | ~258 mm | **95%** |
| **US 8** | US 9.5 | EU 41 | 258 mm | ~266 mm | **98%** |
| **US 9** | US 10.5 | EU 42 | 265 mm | ~273 mm | **100% (Default)** |
| **US 10** | US 11.5 | EU 43 | 273 mm | ~281 mm | **103%** |
| **US 11** | US 12.5 | EU 44 | 280 mm | ~288 mm | **106%** |
| **US 12** | US 13.5 | EU 45 | 288 mm | ~296 mm | **109%** |

> [!NOTE] Diagonal Bed Placement
> For sizes **US 9 and larger**, rotate the shoe **$45^\circ$ diagonally across the build plate** in Bambu Studio to utilize the 362 mm diagonal bed clearance of the X2D.

---

## ⚙️ Slicer Configuration (Bambu Studio)

| Parameter | Recommended Setting | Purpose / Rationale |
| :--- | :--- | :--- |
| **Printer** | Bambu X2D | Direct-drive toolhead handles TPU cleanly |
| **Filament Feed** | **External Spool / 4-in-1 Adapter** | ⚠️ Bypasses AMS 2 Pro to prevent jamming; feeds directly to toolhead |
| **Spool Mount** | **608-Bearing Roller OR Active Dry Box** | Eliminates rotational drag so elastic TPU doesn't stretch thin |
| **Nozzle** | 0.4 mm Hardened Steel | 230°C nozzle temp (or 245°C for Foaming TPU) |
| **Build Plate** | Textured PEI Plate | **Must apply glue stick / liquid glue as a release agent** |
| **Layer Height** | `0.24 mm Draft` or `0.20 mm Standard` | 0.24mm cuts 3–4 hours off total print time |
| **Wall Loops** | `3 walls` (outer) | Provides puncture resistance on pavement |
| **Top / Bottom Layers**| 4 top / 4 bottom layers | Waterproof sole bottom |
| **Infill Pattern** | **Gyroid** | Acts like internal suspension micro-springs |
| **Infill Density** | **12%** | Perfect sweet spot between cushion and support |
| **Supports** | **Tree (Organic) — Auto** | Only for severe overhangs inside the toe box |
| **Max Volumetric Speed** | **$3.5\text{ mm}^3/\text{s}$** | Caps print speed to prevent extruder slipping |

---

## 🧪 Print Run Log

### Left Shoe
* **Date Sliced:** 
* **Scale Applied:** %
* **Filament Spool:** 
* **Estimated Duration:** 
* **Actual Print Time:** 
* **Checklist:**
  - [ ] TPU spool pre-dried at 55°C (6–8 hours); feeding from active dry box or 608-bearing roller.
  - [ ] External PTFE feed tube connected to Bambu 4-in-1 adapter (AMS bypassed).
  - [ ] Textured PEI plate washed with Dawn dish soap, dried, and coated with thin uniform glue barrier.
  - [ ] Model oriented diagonally ($45^\circ$) with sole flat on plate (clearing diagonal bed length).
  - [ ] First layer inspected for uniform squish without popping or bubbling.

### Right Shoe
* **Date Sliced:** 
* **Scale Applied:** % (Mirror of Left Shoe via Slicer `Mirror -> Along X-Axis`)
* **Checklist:**
  - [ ] Model mirrored in slicer.
  - [ ] Fresh thin glue stick layer reapplied to plate for release.
  - [ ] TPU dry box temperature maintained at 50–55°C throughout print.

---

## 💡 Post-Print Finishing & Custom Foot Molding

1. **Support Removal:** Tree supports inside the toe box pop out cleanly with long needle-nose pliers.
2. **Custom Thermal Contouring (Heat Gun / Hot Water Bath):**
   * If the heel strap or instep feels slightly tight, dip the relevant area into a bowl of hot water (~70°C / 160°F) for 30–45 seconds.
   * Put on thick socks, slip your foot into the shoe, and press down onto a flat surface for 60 seconds as it cools. The TPU will permanently conform to your unique foot arch and heel contour!

---

**Parent Index:** [[09 - 3D Printed Footwear (Sneakers, Clogs & TPU)]] | [[08 - Print Queue & Project Tracker]]
