# Awesome Modern Multiple Object Tracking [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, taxonomy-organized index of modern multiple object tracking (MOT) papers, benchmark datasets, and evaluation metrics — the companion resource for the survey *"In Pursuit of Many: A Review of Modern Multiple Object Tracking Systems"* (Machine Intelligence Research, MIR-2026-03-176).

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/iambashar/awesome-mot.svg)](https://github.com/iambashar/awesome-mot/commits)

Every entry is mapped to a section of the survey so the two can be read together. Where a paper ships official code, the row links it and is marked ✅. This list is maintained alongside the survey and updated as the field develops.


## Contents

- [Approach families](#approach-families) — survey Section 3
- [Benchmark datasets](#benchmark-datasets) — survey Section 4
- [Evaluation metrics & toolkits](#evaluation-metrics--toolkits) — survey Section 5
- [Surveys & background](#surveys--background)
- [Contributing](#contributing)
- [Citation](#citation)
- [License](#license)

Legend: ✅ official code available · — no official code located.

## Approach families

Organized by the survey's Section 3 taxonomy, in the same order as the paper. One row per paper.

### 1. Detection and Target Association (tracking-by-detection)

| Paper | Venue / Year | Code |
|---|---|---|
| SORT — Simple Online and Realtime Tracking | ICIP 2016 | ✅ https://github.com/abewley/sort |
| DeepSORT — SORT with a Deep Association Metric | ICIP 2017 | ✅ https://github.com/nwojke/deep_sort |
| ByteTrack — Multi-Object Tracking by Associating Every Detection Box | ECCV 2022 | ✅ https://github.com/ifzhang/ByteTrack |
| OC-SORT — Observation-Centric SORT | CVPR 2023 | ✅ https://github.com/noahcao/OC_SORT |
| FeatureSORT — Robust tracker with optimized feature integration | Machine Vision and Applications 2026 | — |

### 2. Transformers (end-to-end)

| Paper | Venue / Year | Code |
|---|---|---|
| TransTrack — Multiple Object Tracking with Transformer | arXiv 2020 | ✅ https://github.com/PeizeSun/TransTrack |
| TrackFormer — Multi-Object Tracking with Transformers | CVPR 2022 | ✅ https://github.com/timmeinhardt/trackformer |
| MOTR — End-to-End Multiple-Object Tracking with Transformer | ECCV 2022 | ✅ https://github.com/megvii-research/MOTR |
| MOTRv2 — Bootstrapping End-to-End MOT by Pretrained Object Detectors | CVPR 2023 | ✅ https://github.com/megvii-research/MOTRv2 |
| MOTRv3 — Release-Fetch Supervision for End-to-End MOT | arXiv 2023 | — |
| AR-MOT — Autoregressive Multi-object Tracking | arXiv 2026 (2601.01925) | — |

### 3. Motion Models

| Paper | Venue / Year | Code |
|---|---|---|
| MAT — Motion-Aware Tracker | Neurocomputing 2022 | — |
| Compensation Tracker | WACV 2022 | — |
| DiffMOT — Decoupled Diffusion-based Motion Predictor | CVPR 2024 | ✅ https://github.com/Kroery/DiffMOT |

### 4. Graph Models

| Paper | Venue / Year | Code |
|---|---|---|
| MPNTrack — Learning a Neural Solver for Multiple Object Tracking | CVPR 2020 | ✅ https://github.com/dvl-tum/mot_neural_solver |
| DyGLIP — Dynamic Graph for Link Prediction (multi-camera) | CVPR 2021 | ✅ https://github.com/uark-cviu/DyGLIP |
| GSLAMOT — Tracklet & Query Graph (3D) | ACM MM 2024 | — |

### 5. Attention Modules

| Paper | Venue / Year | Code |
|---|---|---|
| FairMOT — On the Fairness of Detection and Re-Identification | IJCV 2021 | ✅ https://github.com/ifzhang/FairMOT |
| MeMOT — Multi-Object Tracking with Memory | CVPR 2022 | — |
| MeMOTR — Long-Term Memory-Augmented Transformer | ICCV 2023 | ✅ https://github.com/MCG-NJU/MeMOTR |
| RelationTrack — Relation-Aware Global Reasoning | IEEE TMM 2022 | — |

### 6. Foundation Models

| Paper | Venue / Year | Code |
|---|---|---|
| Grounding DINO — Open-Vocabulary Detection | ECCV 2024 | ✅ https://github.com/IDEA-Research/GroundingDINO |
| SAM 2 — Segment Anything in Images and Videos | arXiv 2024 | ✅ https://github.com/facebookresearch/sam2 |
| SAMURAI — Zero-shot SAM2-based tracking with motion-aware memory | arXiv 2024 | ✅ https://github.com/yangchris11/samurai |
| SAM2MOT — MOT-by-segmentation on SAM2 | 2025 | — |
| Z-GMOT — Zero-shot Generic MOT | arXiv 2024 (2305.17648) | ✅ https://github.com/Fsoft-AIC/Z-GMOT |
| DINOv2 / DINOv3 — Self-supervised dense backbones | 2023 / 2025 | ✅ https://github.com/facebookresearch/dinov2 |

### 7. Siamese Networks

| Paper | Venue / Year | Code |
|---|---|---|
| Representative online Siamese trackers (survey Sec. 3.7) | 2020–2022 | — |

### 8. Tracklet Association

| Paper | Venue / Year | Code |
|---|---|---|
| Global tracklet linking / re-linking works (survey Sec. 3.8) | 2020–2024 | — |

### 9. Generative (Diffusion) Tracking

| Paper | Venue / Year | Code |
|---|---|---|
| DiffusionTrack — Diffusion Model for Multi-Object Tracking | AAAI 2024 | ✅ https://github.com/RainBowLuoCS/DiffusionTrack |
| DiffMOT — Decoupled Diffusion-based Motion Predictor | CVPR 2024 | ✅ https://github.com/Kroery/DiffMOT |
| Pro2Diff — Proposal Propagation by Diffusion | 2024 | — |
| DiffusionMOT | 2025 | — |

### 10. State Space Models (Mamba)

| Paper | Venue / Year | Code |
|---|---|---|
| MambaTrack — Mamba motion predictor with tracklet patching | 2024 | — |
| MambaMOT — Kalman-filter replacement with Mamba | 2025 | — |
| MambaVLT — Time-evolving multimodal state space (vision-language) | 2025 | — |
| Samba — Synchronized set-of-sequences modeling | 2024 | — |

## Benchmark datasets

Covered in Section 4 of the survey.

| Dataset | Domain | Link |
|---|---|---|
| MOT17 / MOT20 | Pedestrians, crowds | https://motchallenge.net |
| DanceTrack | Uniform appearance, non-linear motion | https://github.com/DanceTrack/DanceTrack |
| SportsMOT | Sports (basketball, volleyball, football) | https://github.com/MCG-NJU/SportsMOT |
| KITTI Tracking | Autonomous driving | https://www.cvlibs.net/datasets/kitti/ |
| nuScenes | 360° multi-modal driving | https://www.nuscenes.org |
| Waymo Open Dataset | Large-scale driving | https://waymo.com/open |
| VisDrone | Aerial / UAV | https://github.com/VisDrone/VisDrone-Dataset |
| BDD100K | Driving, MOT/MOTS | https://www.bdd100k.com |
| TAO | Long-tail, open-world | https://taodataset.org |

## Evaluation metrics & toolkits

Covered in Section 5 of the survey.

| Metric | Defined in | Toolkit |
|---|---|---|
| MOTA / MOTP (CLEAR-MOT) | Bernardin & Stiefelhagen, 2008 | https://github.com/cheind/py-motmetrics |
| IDF1 | Ristani et al., 2016 | py-motmetrics / TrackEval |
| HOTA (DetA, AssA, LocA) | Luiten et al., IJCV 2021 | https://github.com/JonathonLuiten/TrackEval |
| AMOTA / MOTAR | Weng et al., IROS 2020 (adopted by nuScenes) | https://github.com/nutonomy/nuscenes-devkit |
| MOTSA | Voigtlaender et al., CVPR 2019 (MOTS) | https://github.com/JonathonLuiten/TrackEval |

## Surveys & background

- *In Pursuit of Many: A Review of Modern Multiple Object Tracking Systems* — this survey (link upon publication).
- *HOTA: A Higher Order Metric for Evaluating Multi-Object Tracking* — IJCV 2021.
- *DanceTrack: Multi-Object Tracking in Uniform Appearance and Diverse Motion* — CVPR 2022.

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guidelines. In short:

- One row per paper, placed under the approach family it best fits in the survey's taxonomy.
- Include the venue and year; add a code link and the ✅ mark only when official code exists.
- Order entries to match the survey where possible; strict alphabetical order is not required.
- Open a pull request with a one-line rationale for the addition or correction.

## Citation

If this index or the survey helps your work, please cite the survey:


```bibtex
@article{inpursuitofmany2026,
  title   = {In Pursuit of Many: A Review of Modern Multiple Object Tracking Systems},
  journal = {Machine Intelligence Research},
  author = {Bashar, Mk and Islam, Samia and Hussain, Kashifa Kawaakib and Hasan, Md Bakhtiar and Rahman, ABM and Kabir, Md Hasanul},
  year    = {2026},
  note    = {MIR-2026-03-176, to appear}
}
```

> Will update the BibTeX with volume, pages, and DOI once the survey is published.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the maintainers have waived all copyright and related rights to this curated list under [CC0 1.0](LICENSE). Linked papers, code, and datasets remain under their respective licenses.
