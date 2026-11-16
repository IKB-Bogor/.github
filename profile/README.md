<p align="center">
  <img src="https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/ikb-logo.svg" alt="IKB logo" width="160">
</p>

<h1 align="center">IKB · Innovasi Karya Barokah</h1>

<p align="center">
  <b>Digital engineering tools for power transformers and shunt reactors, plus the training and AI platform around them.</b><br>
  <i>Perangkat rekayasa digital untuk trafo daya dan reaktor shunt, beserta platform pelatihan dan AI pendukungnya.</i>
</p>

<p align="center">
  <img alt=".NET 10" src="https://img.shields.io/badge/.NET-10-512BD4?logo=dotnet&logoColor=white">
  <img alt="Avalonia UI" src="https://img.shields.io/badge/Avalonia_UI-11-8B44AC">
  <img alt="Blazor" src="https://img.shields.io/badge/Blazor-Server-5C2D91?logo=blazor&logoColor=white">
  <img alt="Platforms" src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0B1A36">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-22D3EE">
</p>

---

IKB builds modern, cross-platform replacements for the calculation programs and spreadsheets used in
transformer design. Each tool keeps the engineering method of the original, puts it in a tested
calculation engine, and adds a desktop interface with rule checks, charts and reports.

IKB is led by **Didik Susilo**.

## Engineering calculators

| Solution | What it does | Status |
|---|---|---|
| ⚡ **[IKB.CHOC](https://github.com/IKB-Bogor/IKB.CHOC)**<br>Impulse voltage distribution | Calculates how lightning and switching impulses distribute along transformer windings. Windings are modelled as RLC mesh cells (layer, helical, disc, interleaved, shield), waves are fitted to T1/T2, and the solver reports node voltages, differential curves and peak stress per mesh. A .NET reimplementation of the CHOC program. | Released: Windows, macOS, Linux installers |
| 🛢️ **[IKB.DOF](https://github.com/IKB-Bogor/IKB.DOF)**<br>Directed oil flow verification | Checks the ODAF/ODWF cooling of a transformer active part: oil flow split between windings, duct and washer velocities, core leakage, annulus entry speed, winding gradient and the thermal model (hot spot, ageing). Every result is checked against the DH-1-C-2-090/091/092 rules. Includes a live section drawing, a 3D active part view and a printable HTML report. | Released: Windows, macOS, Linux installers |
| 🌀 **[ShuntReactor](https://github.com/IKB-Bogor/ShuntReactor)**<br>Shunt reactor design | Sizes a fixed or variable (VSR) gapped-core shunt reactor from ratings to core gap ladder, winding build, losses, gradient, noise and active material cost. Replaces an 18-sheet Excel workbook and matches all 95 compared quantities of its reference design. | Active development |
| 🌡️ **[IKB.ODAF](https://github.com/IKB-Bogor/IKB.ODAF)**<br>ODAF calculator | Calculator for oil-directed, air-forced (ODAF) transformer cooling. | Planned |

## Platforms

| Solution | What it does |
|---|---|
| 🎓 **[IKB.LMS](https://github.com/IKB-Bogor/IKB.LMS)**<br>Learning management system | Blazor Server LMS for transformer, power system and electrical safety training. Courses, quizzes, exams, gradebook and certificates; course import from PDF, Word, PowerPoint and Excel; AI quiz generation and essay grading that an instructor always reviews; and **Pak Didik**, an in-app AI assistant. Supports OpenAI, Azure OpenAI, Gemini, Anthropic, DeepSeek and Ollama. |
| 🤖 **[IKB_AI](https://github.com/IKB-Bogor/IKB_AI)**<br>AI apps | AI applications for IKB. |

## Screenshots

### ⚡ IKB.CHOC: impulse voltage distribution

| Results: node voltages and stress per mesh | Winding model |
|---|---|
| ![IKB.CHOC results](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/choc-results.png) | ![IKB.CHOC winding model](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/choc-meshes.png) |

### 🛢️ IKB.DOF: directed oil flow verification

| Study overview with live section drawing | Active part in 3D |
|---|---|
| ![IKB.DOF study](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/dof-study.png) | ![IKB.DOF active part 3D](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/dof-active-part-3d.png) |

### 🌀 ShuntReactor: shunt reactor design

| Overview of the design | Winding build |
|---|---|
| ![ShuntReactor overview](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/shuntreactor-overview.png) | ![ShuntReactor windings](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/shuntreactor-windings.png) |

### 🎓 IKB.LMS: learning management system

| Dashboard | Pak Didik, the AI assistant |
|---|---|
| ![IKB.LMS dashboard](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/lms-dashboard.png) | ![IKB.LMS Pak Didik](https://raw.githubusercontent.com/IKB-Bogor/.github/main/assets/screenshots/lms-pak-didik.png) |

## Shared approach

- **One engine, tested.** Calculations live in a core library without UI code and are verified against reference cases from the original program or workbook.
- **Rule checks.** Results are compared with the design rules and shown as PASS / CHECK / FAIL with the rule and the part that failed.
- **Cross-platform.** .NET 10 with Avalonia UI for desktop and Blazor for web; self-contained installers that need no .NET runtime.
- **Bilingual.** Documentation in English and Bahasa Indonesia.
- **Open license.** The calculators are released under the MIT License.

## Contact

Questions or collaboration: open an issue in the relevant repository.

<p align="center"><sub>© 2026 IKB – Innovasi Karya Barokah · Bogor, Indonesia</sub></p>
