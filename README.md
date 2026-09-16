# Integrity Lab

**Integrity Lab** is an interactive engineering application for **mechanics-based and uncertainty-aware structural integrity assessment**. It was developed from my graduate research in Structural Engineering at the University of Alberta to translate research workflows into a practical, inspectable engineering tool.

The application currently focuses on corroded-pipeline assessment and brings deterministic engineering calculations, probabilistic uncertainty propagation, and research-oriented diagnostics into one interface.

## Purpose

Engineering assessment workflows are often split across spreadsheets, research scripts, post-processing notebooks, and model-specific utilities. Integrity Lab was developed to make those workflows easier to explore, reproduce, and communicate through a single application while preserving the underlying mechanics and assumptions.

## Current capabilities

The research release is designed around workflows including:

- **RSTRENG / effective-area assessment** of corrosion profiles;
- **PSQR-based assessment** of two-dimensional corrosion grids;
- propagation of **ILI measurement uncertainty** through Monte Carlo simulation;
- uncertainty-aware failure-pressure distributions and engineering statistics;
- effective corrosion-depth and corrosion-length diagnostics;
- PSQR Axial Alignment Factor (AAF) diagnostics;
- convergence and reproducibility-oriented outputs;
- visualization of engineering inputs, reconstructed profiles, and assessment results.

The application is intended as a research and engineering-analysis platform rather than a replacement for applicable codes, standards, or professional judgment.

## Research background

Integrity Lab grew from the M.Sc. thesis:

> **Seyyed Mohammad Mojtahed Haeri.** *Uncertainty Propagation in Burst-Pressure Assessment of Corroded Pipelines using Engineering and Machine Learning Methods.* University of Alberta, 2026.

Related work includes:

> **S. M. M. Haeri**, S. Attia, K. Shahzad, M. Meleka, S. Abtahi, and S. Adeeb, “Integrating ILI Measurement Uncertainty into the RSTRENG Method via Monte Carlo Simulation,” *ASME Pressure Vessels & Piping Conference (PVP 2026)*, Paper PVP2026-183160, Anaheim, California, 2026.

The underlying research code is being organized separately in:

- [Uncertainty-Aware Structural Assessment](https://github.com/SMmhaeri/Uncertainty-aware-structural-assessment)
- [Probabilistic Structural Machine Learning](https://github.com/SMmhaeri/Probabilistic-structural-ml)

## Packaged application

The complete Windows research build is distributed as a packaged ZIP rather than committing hundreds of megabytes of bundled runtime files directly into Git history.

A packaged release contains application components such as:

```text
IntegrityLab/
├── backend/
├── data/
├── existing_code/
├── frontend/
├── launcher/
├── LICENSES/
├── runtime/
├── IntegrityLab.exe
├── NOTICE.txt
├── product.json
├── READ_ME_FIRST.txt
├── RELEASE_MANIFEST.json
└── TEST_STATUS.txt
```

The full packaged build should be attached to a **GitHub Release** so users can download the application as one ZIP without reconstructing its runtime environment.

## Running the packaged Windows build

1. Download the complete ZIP from the repository's **Releases** page.
2. Extract the entire archive; do not move only `IntegrityLab.exe` out of the extracted directory because the executable may rely on the bundled application structure and runtime.
3. Read `READ_ME_FIRST.txt` included with the package.
4. Launch `IntegrityLab.exe`.

## Data and confidentiality

Integrity Lab was developed in the context of industry-linked research. **Proprietary Enbridge ILI datasets are not intended for public distribution.** Any public release should contain only data that are synthetic, publicly available, or explicitly authorized for redistribution.

Users should independently verify that any datasets they add to the application may legally and contractually be shared.

## Repository status

This repository is being prepared as the public-facing home of Integrity Lab. The packaged application, screenshots, technical documentation, and source components will be added in stages after release and IP checks.

## License and reuse

A public software license has **not yet been assigned**. The presence of files in this repository does not by itself grant permission to reuse proprietary or third-party components. Bundled third-party notices and licenses supplied with the application should be preserved.

## Author

**Mohammad Haeri**  
M.Sc. Researcher in Structural Engineering, University of Alberta  
[LinkedIn](https://linkedin.com/in/smmhaeri) · [GitHub](https://github.com/SMmhaeri) · [Email](mailto:sm.mojtahed@gmail.com)
