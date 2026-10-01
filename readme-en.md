# Desmos‑Based Animation Design Assistant Toolkit
This project is a set of **custom function libraries for Desmos**. It encapsulates a large number of pre‑built functions for quickly creating geometric animations, particle effects and parametric graphics within the Desmos Graphing Calculator, streamlining animation‑creation workflows.

### 🎬 [Project Link (full library pre‑loaded for direct experimentation)](https://www.desmos.com/geometry/nsi2zipg3w)

### ⚠️ Important Document Risk Notice
> The Chinese user manual was AI‑assisted. Although proofread against the original source code, textual descriptions, formula interpretations and examples may still contain deviations, typos or misinterpretations compared with actual source‑code behaviour.

- Whenever there is a conflict between documentation descriptions and the behaviour given in the raw source file `基本参数 rd260925.txt`, **the runtime output from the pre‑configured online Desmos project shall be the sole authoritative reference**.
- For critical features and key parameters, verify behaviour directly against the source code or the online project; do not rely entirely on written documentation.
- The translated English‑language PDF manual is derived from the AI‑assisted Chinese document and carries the same potential risk of inaccuracy.

### 📁 Repository File Inventory

| Filename | Description |
|---|---|
| Desmos Custom Function Library User Manual.pdf | English‑language user‑manual PDF, translated from the Chinese document for international users. Subject to potential inaccuracies introduced by AI translation. |
| Desmos 自定义函数库使用说明 rd‑261001.docx | ✅【Recommended】Full‑featured Chinese documentation: function parameters, invocation examples and notes.<br>💡 Microsoft Word is recommended for best rendering of formulas and layouts.<br>⚠️ AI‑assisted content; cross‑validate against source code. |
| Desmos 自定义函数库使用说明 rd‑261001.pdf | PDF fallback copy of the Chinese `.docx` manual; shares the same potential inaccuracies of AI‑assisted documentation. |
| README.md | Repository read‑me file (this document). |
| 基本参数 rd260925.txt | Use this file to copy‑paste LaTeX definitions into the Desmos expression panel if you cannot open the online project link. |

### ✨ Library Feature Overview
This custom function library provides a comprehensive set of utility functions:
- Geometry drawing: arbitrary‑order Bézier curves, piecewise cubic Bézier curves, polar‑coordinate transformations, parametric circles and more
- Particle system: region‑bound random‑particle generation, particle motion with wrap‑around boundaries
- Numeric utilities: value clamping, interval normalisation, cyclic wrapping, linear interpolation
- Random‑number utilities: seed‑controlled random‑value lists, sequence generation
- List utilities: list insertion, deletion, replacement, index lookup
- Animation & easing: 30+ built‑in easing functions; single‑segment and multi‑segment chained animations
- Advanced utilities: matrix reshaping, list‑mapping templates

### 🎯 Intended Audience
- Creators building mathematical animations and parametric graphics inside Desmos
- Users who want particle‑system, Bézier‑curve and easing‑driven animations without writing low‑level expressions manually
- Enthusiasts for teaching demonstrations, video animations and geometric visualisation

### 📌 Critical Usage Notes
1. Desmos lists use **1‑based indexing; index 0 does not exist**. Keep this in mind when writing expressions.
2. This library contains no built‑in parameter validation. Illegal inputs or mismatched list lengths may trigger errors or return empty results.
3. Point‑lists cannot be fed directly into functions expecting numeric‑value lists. Split coordinates via `.x` / `.y`, process each numeric list separately, then reconstruct point objects afterwards.

### ❓ Frequently Asked Questions

#### Q: Why is Microsoft Word recommended for opening the `.docx` file?
A: The document contains extensive formulas and tables. Minor layout misalignment can appear in PDF exports; Microsoft Word renders formulas and layouts correctly.
If obvious formatting corruption occurs in the `.docx`, please use the corresponding `.PDF` file instead.

#### Q: Documented behaviour differs from actual runtime results. What should I do?
Check the following items in sequence:
- Confirm complex‑number mode is disabled
- Verify that **radian mode** is enabled (found inside the wrench‑icon settings in the upper‑right corner)
- Please open an Issue to report documentation defects or runtime‑behaviour bugs.

### 📜 Version Information
- Version identifier: rd261001
- Base source‑code version: rd260925
- Revision date: 2026‑10‑01

### 📄 Licence Statement
You are free to use and modify this source code for personal‑learning and non‑commercial creative purposes.

### 📫 Feedback & Contributions
Report bugs, documentation errors or feature suggestions by opening repository Issues.
