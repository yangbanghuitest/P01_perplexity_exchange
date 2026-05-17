# Cleaned Verified References Patch Plan

Source CSV: `03_candidate_reference_tables/verified_references_30_20260511_085129.csv`
Cleaned CSV: `03_candidate_reference_tables/verified_references_30_cleaned_20260511_085359.csv`
Cleaned workbook: `03_candidate_reference_tables/verified_references_30_cleaned_20260511_085359.xlsx`
Screening workbook: `04_screening_decisions/screening_decisions_verified_30_cleaned_20260511_085359.xlsx`

## Counts

- Must cite: 18
- Supplement only: 8
- Background only: 4
- Needs manual check: 15

## Must-Cite References

| ID | Reference | DOI | Section | Issues | Metadata |
|---|---|---|---|---|---|
| R01 | Fadilah, W.A.; Murtiyoso, A.; Landes, T.; Grussenmeyer, P. (2026). Metric Assessment of 3D Gaussian Splatting for UAV-Based Urban Heritage Reconstruction. ISPRS Archives XLVIII-2/W12-2026 | 10.5194/isprs-archives-XLVIII-2-W12-2026-143-2026 | Sec 1.2; Sec 4; Sec 5 | F1; F6; F11 | Verified |
| R02 | Savant Aira, L.; Facciolo, G.; Ehret, T. (2025). Gaussian Splatting for Efficient Satellite Image Photogrammetry (EOGS). CVPR 2025 (also arXiv:2412.13047) | 10.48550/arXiv.2412.13047 | Sec 2; Sec 5 | F1; F6; F11 | Verified – formal venue is CVPR 2025 |
| R03 | Haitz, D.; Hermann, M.; Solana Roth, A.; Weinmann, M.; Jutzi, B. (2024). The Potential of Neural Radiance Fields and 3D Gaussian Splatting for 3D Reconstruction from Aerial Imagery. ISPRS Annals X-2-2024 | 10.5194/isprs-annals-X-2-2024-97-2024 | Sec 1.2; Sec 4 | F1; F6; F11 | Verified |
| R05 | He, Z.; et al. (2025). Dynamic Urban Scene Modeling with 3D Gaussian Splatting from UAV Full-Motion Videos. ISPRS Archives XLVIII-G-2025 | 10.5194/isprs-archives-XLVIII-G-2025-649-2025 | Sec 5 | F1; F6; F11 | Partial – full author list needs ISPRS page check |
| R07 | Marí, R.; de Franchis, C.; Meinhardt-Llopis, E.; Anger, J.; Facciolo, G. (2021). A Generic Bundle Adjustment Methodology for Indirect RPC Model Refinement of Satellite Imagery. Image Processing On Line 11 | 10.5201/ipol.2021.352 | Sec 2 | F1; F2; F11 | Verified |
| R08 | Dong, Y.; Lei, R.; Fan, D.; Gu, L.; Ji, S. (2020). A Novel RPC Bias Model for Improving the Positioning Accuracy of Satellite Images. ISPRS Annals V-2-2020 | 10.5194/isprs-annals-V-2-2020-35-2020 | Sec 2 | F1; F6; F11 | Verified |
| R09 | Cao, K.; Li, J.; Song, R.; Liu, Z.; Li, Y. (2024). Model-Driven Deep Pipeline With Uncertainty-Aware Bundle Adjustment for Satellite Photogrammetry. IEEE Trans. Geoscience and Remote Sensing 62:5605313 | 10.1109/TGRS.2024.3352072 | Sec 2; Sec 4 | F1; F2; F11 | Verified |
| R10 | Jiang, N.; Li, H.; Li, C.; Hu, Y.; Zhou, J. (2025). Bundle Adjustment-Based Co-Registration with High Geolocation Accuracy for Multi-Temporal UAV Data. ISPRS JPRS (online 2025) | 10.1016/j.isprsjprs.2025.11.014 | Sec 2 | F1; F6; F11 | Verified |
| R11 | Liu, Y.; et al. (2025). Influence of Ground Control Point Reliability and Distribution on UAV Photogrammetric 3D Mapping Accuracy. Geo-spatial Information Science | 10.1080/10095020.2025.2451204 | Sec 2; Sec 4 | F1; F2; F6; F11 | Partial – full author list pending |
| R12 | Štroner, M.; Urban, R.; Seidl, J.; Reindl, T.; Broucek, J. (2021). Photogrammetry Using UAV-Mounted GNSS RTK: Georeferencing Strategies without GCPs. Remote Sensing 13(7):1336 | 10.3390/rs13071336 | Sec 2 | F1; F2; F11 | Verified |
| R14 | Elkhrachy, I. (2021). Accuracy Assessment of Low-Cost Unmanned Aerial Vehicle (UAV) Photogrammetry. Alexandria Engineering Journal 60(6) | 10.1016/j.aej.2021.07.022 | Sec 4 | F1; F6; F11 | Verified |
| R15 | Simard, M.; Denbina, M.; Marshak, C.; Neumann, M. (2024). A Global Evaluation of Radar-Derived Digital Elevation Models: SRTM, NASADEM, and GLO-30. Journal of Geophysical Research: Biogeosciences 129:e2023JG007672 | 10.1029/2023JG007672 | Sec 4 | F1; F6; F11 | Verified |
| R17 | Rabiu, A.A.; Ahmad, A. (2023). UAV Photogrammetric Products Accuracy Assessment: A Review. ISPRS Archives XLVIII-4/W6-2022 | 10.5194/isprs-archives-XLVIII-4-W6-2022-279-2023 | Sec 1.2 | F1; F3; F6; F11 | Verified |
| R19 | Nguyen, V.M.; Sandidge, E.; Mahendrakar, T.; White, R.T. (2024). Characterizing Satellite Geometry via Accelerated 3D Gaussian Splatting. Aerospace (MDPI) 11(3):183 | 10.3390/aerospace11030183 | Sec 5 | F1; F11 | Verified |
| R22 | Page, M.J.; McKenzie, J.E.; Bossuyt, P.M.; Boutron, I.; Hoffmann, T.C.; Mulrow, C.D.; Shamseer, L.; et al.; Moher, D. (2021). The PRISMA 2020 Statement: An Updated Guideline for Reporting Systematic Reviews. BMJ 372:n71 | 10.1136/bmj.n71 | Sec 1.2 | F11; F12 | Verified |
| R23 | Page, M.J.; Moher, D.; Bossuyt, P.M.; Boutron, I.; Hoffmann, T.C.; Mulrow, C.D.; et al. (2021). PRISMA 2020 Explanation and Elaboration: Updated Guidance and Exemplars for Reporting Systematic Reviews. BMJ 372:n160 | 10.1136/bmj.n160 | Sec 1.2 | F11; F12 | Verified |
| R24 | Zhu, Y.; et al. (2025). Ortho-3DGS: True Digital Orthophoto Generation from UAV Imagery Using Depth-Regulated 3D Gaussian Splatting. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing | 10.1109/JSTARS.2025.3557540 | Sec 4; Sec 5 | F1; F6; F11 | Partial – first author needs IEEE Xplore confirmation |
| R30 | Hermann, M.; Weinmann, M.; Nex, F.; Stathopoulou, E.K.; Remondino, F.; Jutzi, B.; Ruf, B. (2024). Depth Estimation and 3D Reconstruction from UAV-Borne Imagery: Evaluation on the UseGeo Dataset. ISPRS Open Journal of Photogrammetry and Remote Sensing 100065 | 10.1016/j.ophoto.2024.100065 | Sec 1.2; Sec 4 | F1; F6; F11 | Partial – DOI inferred from UseGeo page citation; verify before submission |

## Section-Level Integration

### Sec 1.2

- `R01`: Geometric accuracy ≠ rendering quality; UAV nadiral 3DGS at 80 m; RMSE/Chamfer on heritage
- `R03`: COLMAP vs Nerfacto vs Splatfacto on nadir aerial UAV (UseGeo dataset); RMSE/Chamfer comparison
- `R17`: Review of DEM accuracy parameters: flying height, overlap, GCP density, LiDAR comparison
- `R22`: 27-item PRISMA checklist; flow diagram for systematic reviews; inclusion/exclusion reporting
- `R23`: Exemplars for each PRISMA item; evidence coding guidance; flow diagram elaboration
- `R30`: UAV depth estimation benchmark; NeRF/MVS/3DGS comparison; UseGeo dataset completeness/correctness

### Sec 2

- `R02`: RPC/affine camera model integrated into 3DGS; radiometric correction; satellite DSM generation
- `R07`: RPC bias correction; tie-point bundle adjustment; error propagation for satellite stereo pairs
- `R08`: Object-space RPC bias correction; full-link error analysis; GCP-free satellite positioning
- `R09`: Uncertainty-aware BA; error propagation modelling; deep learning integration with physical model
- `R10`: Multi-temporal UAV SfM BA co-registration; GCP-aided alignment; checkpoint residuals
- `R11`: GCP RMSE residuals; 15 configurations; error propagation from GCP reliability to DSM accuracy
- `R12`: GNSS RTK direct georeferencing; systematic elevation error from focal length deviation; error propagation

### Sec 4

- `R01`: Geometric accuracy ≠ rendering quality; UAV nadiral 3DGS at 80 m; RMSE/Chamfer on heritage
- `R03`: COLMAP vs Nerfacto vs Splatfacto on nadir aerial UAV (UseGeo dataset); RMSE/Chamfer comparison
- `R09`: Uncertainty-aware BA; error propagation modelling; deep learning integration with physical model
- `R11`: GCP RMSE residuals; 15 configurations; error propagation from GCP reliability to DSM accuracy
- `R14`: RMSE for horizontal/vertical; GCP vs direct georeferencing; ASPRS 2015 accuracy standards
- `R15`: Global DEM RMSE, bias per terrain class; GEDI/ICESat-2 validation; completeness/correctness
- `R24`: Depth-regulated 3DGS for orthoimage; geometric accuracy metrics; RS product generation
- `R30`: UAV depth estimation benchmark; NeRF/MVS/3DGS comparison; UseGeo dataset completeness/correctness

### Sec 5

- `R01`: Geometric accuracy ≠ rendering quality; UAV nadiral 3DGS at 80 m; RMSE/Chamfer on heritage
- `R02`: RPC/affine camera model integrated into 3DGS; radiometric correction; satellite DSM generation
- `R05`: Dynamic 3DGS + photogrammetric initialisation; UAV video; urban scene Chamfer/normal metrics
- `R19`: On-orbit 3DGS for RSO geometry; hardware-in-loop; spaceflight hardware compute constraints
- `R24`: Depth-regulated 3DGS for orthoimage; geometric accuracy metrics; RS product generation

## Manual Checks Before Main-Text Integration

| ID | Title | Status | Reason |
|---|---|---|---|
| R02 | Gaussian Splatting for Efficient Satellite Image Photogrammetry (EOGS) | Verified – formal venue is CVPR 2025 | Only published work adapting 3DGS to full satellite RPC pipeline; seminal for RS–3DGS bridge |
| R05 | Dynamic Urban Scene Modeling with 3D Gaussian Splatting from UAV Full-Motion Videos | Partial – full author list needs ISPRS page check | Only ISPRS-venue dynamic 3DGS paper integrating photogrammetric pipeline; directly relevant to RS digital twins |
| R06 | HyGS-TDOM: A Hybrid Gaussian Splatting Framework for Generating True Digital Orthophoto Maps from UAV Images | Partial – full author list needs ISPRS page check | Relevant for RS orthophoto digital twins but niche; include if Section 5 covers products |
| R11 | Influence of Ground Control Point Reliability and Distribution on UAV Photogrammetric 3D Mapping Accuracy | Partial – full author list pending | Systematic GCP-error propagation study; fills Sec 2 gap on checkpoint residuals |
| R13 | Real-Time Bundle Adjustment for Ultra-High-Resolution UAV Imagery Using Adaptive Patch-Based Feature Tracking | Partial – full author list needs verification | Relevant to Sec 2 but focuses on UAV only; include if review discusses airborne BA efficiency |
| R20 | Improved 3D Gaussian Splatting of Unknown Spacecraft Structure Using Space Environment Illumination Knowledge | Preprint – no formal DOI found; IEEE proceedings DOI pending | Supplements R19 with illumination-aware aerospace 3DGS; cite after confirming IEEE proceedings DOI |
| R21 | SkySplat: Generalizable 3D Gaussian Splatting from Multi-Temporal Sparse Satellite Images | Preprint – use with caution; no peer-reviewed venue confirmed | Strong technical contribution but preprint only; promote to Must cite if published before submission |
| R22 | The PRISMA 2020 Statement: An Updated Guideline for Reporting Systematic Reviews | Verified | Canonical reference for reproducible review methodology; required for ISPRS JPRS review papers |
| R23 | PRISMA 2020 Explanation and Elaboration: Updated Guidance and Exemplars for Reporting Systematic Reviews | Verified | Companion to R22; provides evidence coding templates and exemplars for technical RS reviews |
| R24 | Ortho-3DGS: True Digital Orthophoto Generation from UAV Imagery Using Depth-Regulated 3D Gaussian Splatting | Partial – first author needs IEEE Xplore confirmation | IEEE JSTARS venue; direct RS product (TDOM) from 3DGS; strengthens Sec 4 metric discussion |
| R25 | TOrtho-Gaussian: Splatting True Digital Orthophoto Maps | Preprint | Closely related to R24; include only if published; avoid citing two near-identical preprints |
| R26 | A Review of Digital Processing of Historical Aerial and Satellite Stereo Imagery | No DOI found – HAL preprint only | Useful background on satellite stereo history but no confirmed DOI; defer to published version |
| R27 | A Survey on Surface Reconstruction Based on 3D Gaussian Splatting | Verified | CV-oriented survey; use in Sec 1.2 only to contrast with RS-focused scope of review |
| R29 | High-Quality Spatial Reconstruction and Orthoimage Generation Using Efficient 2D Gaussian Splatting | Preprint | Relevant to orthophoto production in digital twins; promote to Must cite if published |
| R30 | Depth Estimation and 3D Reconstruction from UAV-Borne Imagery: Evaluation on the UseGeo Dataset | Partial – DOI inferred from UseGeo page citation; verify before submission | Directly links RS UAV reconstruction evaluation to RS-grade metrics; UseGeo dataset used in R03 |
