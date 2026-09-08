# 🤖 Agent Operational Guidelines & Repository Rules

Welcome, Agent. This repository defines the digital manufacturing notes, slicer configurations, engineering standards, and physical workshop organization projects for 3D printing (specifically tailored to the **Bambu X2D** dual-extrusion ecosystem).

When assisting in this repository or creating/modifying documentation, you **MUST** strictly adhere to the following rules:

---

## 1. 🚫 Git Commit & Push Policy (Absolute Rule)

* **Assist with Commit Messages**: When tasks or file modifications are complete, suggest clear, well-structured commit messages following the Conventional Commits standard.
* **DO NOT Commit or Push Changes**: Under **NO circumstances** should the agent execute `git commit` or `git push`.
* **User Authority**: Only the **USER** is authorized to review diffs, stage files, commit, and push to version control.

---

## 2. 📝 Documentation & Linking Rules (Obsidian & GitHub Scope)

* **Strict Repository Self-Containment**: All links within this repository MUST resolve exclusively to notes and files inside `3d-printing`. Never generate relative links that traverse out to sibling directories or other repositories (e.g., do NOT write `[[../nix-mac/...]]` or `[...](../talos-aws-homelab/...)`).
* **Obsidian Wikilinks Standard**: Use standard Obsidian Wikilinks `[[Note Name]]` (or `[[Folder/Note Name|Display Text]]`) for all internal note cross-references, filament guides, and project logs.
* **External Cross-References**: If you need to reference an external project, tool, or sibling repository, mention it in plain text or provide the full canonical GitHub URL—never a relative local file path.

---

## 3. 🏛️ Engineering & Manufacturing Standards

* **Bambu X2D Hardware Specifics**:
  * Dual independent hotends (300°C) with active heated chamber (65°C).
  * True zero-gap support interfaces (`Support for ABS` with ASA; PETG with PLA).
  * External PTFE feed bypass for TPU 95A / foaming TPU (never feed soft TPU through AMS).
* **Workshop Organization Hierarchy**:
  * **Level 1 (Macro)**: 3/4" Baltic Birch French Cleats (universal 45° wall rails).
  * **Level 2**: Multiboard Islands (removable wall tool clusters).
  * **Level 3 (Micro)**: Gridfinity (42mm open standard for drawers/trays) and Underware on Multiboard tiles.
* **Material Selection Discipline**:
  * Outdoor / High-Heat / Load-bearing: ASA or EZ PA Nylon.
  * Wearables / Ergonomics: TPU 95A / Foaming varioShore TPU.
  * Ultra-precision / 0.2mm Hotend: High-flow PLA / PETG with sequential object-by-object printing.

---

## 4. 📂 Project Logging & Template Standards

* **New Build Documentation**: Every substantive print project must have a dedicated log inside `Projects/` using the schema defined in `Templates/Template - Print Project Log.md`.
* **Filament Tracking**: Track spools, drying temperatures, and densities using `Templates/Template - Filament Spool Tracker.md`.
* **Metadata Frontmatter**: Maintain consistent YAML frontmatter at the top of notes (`title`, `tags`, `created`, `updated`, `category`).

---

## 5. 📝 Conventional Commits Standard

When proposing commit messages to the user:
* Format: `<type>(<scope>): <description>`
* Common scopes: `bambu`, `slicer`, `cleats`, `multiboard`, `gridfinity`, `footwear`, `keycaps`, `materials`, `docs`.
* Examples:
  * `docs(materials): update ASA drying chamber temperature guidelines`
  * `feat(footwear): add parametric clog slicing recipe for TPU 95A`
