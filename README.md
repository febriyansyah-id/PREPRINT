# PREPRINT

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](./LICENSE)
[![Status](https://img.shields.io/badge/Status-Preprint-blue.svg)](#publications)
[![Archive](https://img.shields.io/badge/Archive-Zenodo-1682D4.svg)](https://zenodo.org/search?q=Febriyansyah)

A curated collection of preprints by **Febriyansyah**, each archived on Zenodo with a persistent DOI. This repository holds the PDF manuscripts together with a structured index of their metadata, abstracts, and citation details.

> **Note.** The works listed here are preprints. They have not been peer reviewed. Please cite the version and DOI you consult.

---

## Contents

- [Publications](#publications)
  - [1. Accuracy–Efficiency Trade-off of ResNet18 and MobileNetV4](#1-accuracyefficiency-trade-off-of-resnet18-and-mobilenetv4)
  - [2. Enterprise Storage in 2026](#2-enterprise-storage-in-2026)
- [Repository structure](#repository-structure)
- [How to cite](#how-to-cite)
- [License](#license)
- [Contact](#contact)

---

## Publications

| # | Title | Date | Type | DOI |
|:-:|---|:-:|:-:|---|
| 1 | Accuracy–Efficiency Trade-off of ResNet18 and MobileNetV4 for Image-Based Malware Family Classification on the Malimg Dataset | 2026-11-26 | Preprint | [10.5281/zenodo.24553437](https://doi.org/10.5281/zenodo.24553437) |
| 2 | Enterprise Storage in 2026: A Multivocal Review of Vendors for AI, Cyber Resilience, and Hybrid Cloud | 2026-11-24 | Preprint | [10.5281/zenodo.24496270](https://doi.org/10.5281/zenodo.24496270) |

---

### 1. Accuracy–Efficiency Trade-off of ResNet18 and MobileNetV4

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.24553437-1682D4.svg)](https://doi.org/10.5281/zenodo.24553437)
· [PDF](./docs/papers/Accuracy-Efficiency_Trade-off_ResNet18_MobileNetV4_Malimg.pdf)
· [Zenodo record](https://zenodo.org/records/24553437)

<details>
<summary><strong>Abstract</strong> (click to expand)</summary>

<br>

Image-based malware classification on the Malimg dataset commonly reports accuracies close to 100%, but computational cost is rarely reported in a comparable way. We compare ResNet18, MobileNetV4-Conv-Small, and MobileNetV4-Conv-Medium, all initialised from ImageNet weights, under a single controlled protocol. After removing 1,330 exact duplicate images and excluding two families with fewer than ten unique images, we use 8,001 images in 23 families with a stratified 70/15/15 split (5,600 / 1,200 / 1,201). Each model is trained with fine-tuning and with feature extraction using three seeds (18 runs). Macro-F1 is the primary metric; efficiency is measured by parameter count, model size, GFLOPs, CPU and GPU latency, training time, and peak GPU memory.

</details>

<details>
<summary><strong>Key results</strong> (click to expand)</summary>

<br>

| Model (fine-tuned) | Test macro-F1 (mean ± sd, 3 seeds) |
|---|:-:|
| ResNet18 | 0.9789 ± 0.0041 |
| MobileNetV4-Conv-Small | 0.9755 ± 0.0018 |
| MobileNetV4-Conv-Medium | 0.9740 ± 0.0053 |

- The F1 gaps between models are within seed-to-seed variation.
- **MobileNetV4-Small** uses 4.4× fewer parameters, 9.8× fewer GFLOPs, and has 2.5× lower CPU latency than ResNet18. A GPU latency advantage was not demonstrated.
- **MobileNetV4-Medium** is dominated by MobileNetV4-Small on every measured metric.
- Fine-tuning is consistently better than feature extraction.

*Scope:* the findings are descriptive. They are based on one dataset, three seeds, and a Kaggle environment.

</details>

<details>
<summary><strong>Keywords</strong></summary>

<br>

`malware classification` · `Malimg` · `ResNet18` · `MobileNetV4` · `accuracy–efficiency trade-off`

</details>

---

### 2. Enterprise Storage in 2026

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.24496270-1682D4.svg)](https://doi.org/10.5281/zenodo.24496270)
· [PDF](./docs/papers/Enterprise_Storage_2026_Multivocal_Review.pdf)
· [Zenodo record](https://zenodo.org/records/24496270)

<details>
<summary><strong>Abstract</strong> (click to expand)</summary>

<br>

This preprint presents a **Multivocal Literature Review (MLR)** of the enterprise storage landscape as of late 2026. It follows the guidelines of Garousi et al. (2019) with adapted PRISMA 2020 reporting. The review combines peer-reviewed literature with grey literature (vendor documentation, analyst reports, and independent benchmarks such as SPC, SPECstorage, MLPerf Storage, and IO500) published between January 2024 and November 2026.

The scope covers primary block storage, scale-out file/NAS, object storage, software-defined storage (SDS), and Storage-as-a-Service (STaaS). Vendors reviewed include Hitachi Vantara, Dell Technologies, NetApp, Pure Storage, HPE, IBM, Huawei, Lenovo, Infinidat, and Fujitsu, with briefer coverage of AI/HPC and SDS specialists such as VAST Data, DDN, and WEKA. Vendor performance claims are explicitly distinguished from independent benchmark results.

</details>

<details>
<summary><strong>Research questions</strong> (click to expand)</summary>

<br>

| ID | Question |
|:-:|---|
| RQ1 | What are the main technology trends in enterprise storage in 2024–2026? |
| RQ2 | How do leading vendors compare across architecture, performance, cyber resilience, AI readiness, hybrid cloud, management/AIOps, and consumption model? |
| RQ3 | How is Hitachi Vantara positioned relative to other vendors, based on available evidence? |
| RQ4 | What are the implications for organizations selecting a storage platform, including in Southeast Asia and Indonesia? |

</details>

<details>
<summary><strong>Keywords</strong></summary>

<br>

`enterprise storage` · `multivocal literature review` · `cyber resilience` · `AI infrastructure` · `hybrid cloud` · `software-defined storage` · `storage-as-a-service`

</details>

> *This is a preprint and has not been peer reviewed. Product and company names are trademarks of their respective owners. AI-assisted tools were used for literature search and drafting; all content was reviewed and verified by the author.*

---

## Repository structure

```text
PREPRINT/
├── docs/                                            # GitHub Pages site (landing pages + PDFs)
│   ├── Accuracy-Efficiency_Trade-off_ResNet18_MobileNetV4_Malimg.pdf
│   └── Enterprise_Storage_2026_Multivocal_Review.pdf
├── .zenodo.json                                     # Zenodo metadata
├── CITATION.cff                                     # Citation metadata (CFF)
├── LICENSE                                          # CC BY 4.0
└── README.md
```

---

## How to cite

Cite the specific work you use. The BibTeX entries below use the Zenodo DOIs.

<details>
<summary><strong>BibTeX: Accuracy–Efficiency Trade-off (ResNet18 / MobileNetV4)</strong></summary>

<br>

```bibtex
@misc{febriyansyah2026accuracy,
  author       = {Febriyansyah},
  title        = {Accuracy--Efficiency Trade-off of ResNet18 and MobileNetV4 for Image-Based Malware Family Classification on the Malimg Dataset},
  year         = {2026},
  howpublished = {Zenodo},
  doi          = {10.5281/zenodo.24553437},
  note         = {Preprint}
}
```

</details>

<details>
<summary><strong>BibTeX: Enterprise Storage in 2026</strong></summary>

<br>

```bibtex
@misc{febriyansyah2026storage,
  author       = {Febriyansyah},
  title        = {Enterprise Storage in 2026: A Multivocal Review of Vendors for AI, Cyber Resilience, and Hybrid Cloud},
  year         = {2026},
  howpublished = {Zenodo},
  doi          = {10.5281/zenodo.24496270},
  note         = {Preprint}
}
```

</details>

---

## License

The manuscripts and metadata are released under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](./LICENSE). You may share and adapt the material, including for commercial purposes, provided you give appropriate credit.

---

## Contact

**Febriyansyah** · Research & Engineering
For questions about the content, open a GitHub issue in this repository.

<div align="center">

[![Zenodo](https://img.shields.io/badge/Zenodo-Author%20profile-1682D4?logo=zenodo&logoColor=white)](https://zenodo.org/search?q=Febriyansyah)

</div>
