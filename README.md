# Integrity Lab

**Integrity Lab** is an interactive engineering application for **mechanics-based and uncertainty-aware structural integrity assessment**. It was developed from graduate research in Structural Engineering at the University of Alberta to translate research workflows into a practical and inspectable engineering tool.

The current research release focuses on corroded-pipeline assessment and brings deterministic engineering calculations, probabilistic uncertainty propagation, and research-oriented diagnostics into one interface.

## Purpose

Engineering assessment workflows are often distributed across spreadsheets, research scripts, post-processing notebooks, and model-specific utilities. Integrity Lab brings these components into a single application while preserving the mechanics, assumptions, and uncertainty structure of the underlying assessment methods.

## Current capabilities

The application supports research workflows including:

- **RSTRENG / effective-area assessment** of corrosion profiles;
- **PSQR-based assessment** of two-dimensional corrosion grids;
- propagation of **ILI measurement uncertainty** through Monte Carlo simulation;
- uncertainty-aware failure-pressure distributions and engineering statistics;
- effective corrosion-depth and corrosion-length diagnostics;
- PSQR Axial Alignment Factor (AAF) diagnostics;
- convergence and reproducibility-oriented outputs;
- visualization of engineering inputs, reconstructed profiles, and assessment results.

Integrity Lab is a research and engineering-analysis platform. It is not a replacement for applicable codes, standards, qualified engineering review, or professional judgment.

## Research background

Integrity Lab grew from the M.Sc. thesis:

> **Seyyed Mohammad Mojtahed Haeri.** *Uncertainty Propagation in Burst-Pressure Assessment of Corroded Pipelines using Engineering and Machine Learning Methods.* University of Alberta, 2026.

Related work includes:

> **S. M. M. Haeri**, S. Attia, K. Shahzad, M. Meleka, S. Abtahi, and S. Adeeb, “Integrating ILI Measurement Uncertainty into the RSTRENG Method via Monte Carlo Simulation,” *ASME Pressure Vessels & Piping Conference (PVP 2026)*, Paper PVP2026-183160, Anaheim, California, 2026.

Research implementations are documented separately in:

- [Uncertainty-Aware Structural Assessment](https://github.com/SMmhaeri/uncertainty-aware-structural-assessment)
- [Probabilistic Structural Machine Learning](https://github.com/SMmhaeri/probabilistic-structural-ml)

## Packaged application

The complete Windows research build is distributed through **GitHub Releases** rather than committing hundreds of megabytes of bundled runtime files to Git history.

### v1.0.0 research pre-release

The current packaged build is available as `IntegrityLab.zip` on the repository's Releases page. The archive is approximately 527 MiB and contains the application together with its bundled runtime and supporting files.

For integrity checking, the uploaded release asset has SHA-256 digest:

```text
340db243570d7e04b32b964789483986afd19e28b79d2a12cf954ec3574ce383
```

The packaged distribution contains components such as:

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

## Running the packaged Windows build

1. Download `IntegrityLab.zip` from the repository's **Releases** page.
2. Extract the complete archive. Do not move only `IntegrityLab.exe` out of the extracted directory because the executable relies on the bundled application structure and runtime.
3. Read `READ_ME_FIRST.txt` included with the package.
4. Launch `IntegrityLab.exe`.

## Data and confidentiality

Integrity Lab was developed in the context of industry-linked research. Repository and release materials intended for public distribution should contain only synthetic, publicly available, or explicitly authorized data. Proprietary inspection data and other restricted industry material should remain outside the public repository.

Users are responsible for ensuring that datasets they add to the application may be used and shared under the applicable legal, contractual, and organizational requirements.

## License and reuse

A public software license has **not yet been assigned**. Publication of this repository or release does not by itself grant reuse rights beyond those provided by applicable law and GitHub's terms. Third-party notices and licenses supplied with the packaged application should be preserved.

## Author

**Mohammad Haeri**  
M.Sc. Researcher in Structural Engineering, University of Alberta  
[LinkedIn](https://linkedin.com/in/smmhaeri) · [GitHub](https://github.com/SMmhaeri) · [Email](mailto:sm.mojtahed@gmail.com)
