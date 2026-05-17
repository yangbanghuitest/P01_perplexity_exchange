# Tables 2 and 3 — ISPRS JPRS Review v2

*For:* 3D Gaussian Splatting from Remote Sensing Reconstruction to Aerospace Digital Twins: A Multi-source Fusion Review for Final-Assembly Smart Factories

---

## Table 2: Quantitative Comparison of Representative Remote-Sensing and Aerial 3DGS Methods

> **Note on reference numbering.** Citations follow the v1 corpus numbering ([6], [8], etc.) and the Addendum placeholders ([A5], [B1], [B4]). These will be resolved to sequential integers upon final bibliography merge.

| Method | Year | Venue | Sensor | Scene scale | PSNR (dB) | SSIM | Geometric accuracy | Dataset | Code |
|---|---|---|---|---|---|---|---|---|---|
| 3DGS [6] | 2023 | ACM SIGGRAPH / TOG | RGB camera | Object / bounded outdoor | 27.21 | 0.815 | Photometric only | Mip-NeRF 360 | yes |
| Mip-Splatting [A5] | 2024 | CVPR (Best Student Paper) | RGB camera | Bounded outdoor (multi-scale) | 27.79 | 0.827 | Photometric only | Mip-NeRF 360 (single-scale test) | yes |
| Mega-NeRF [B4] | 2022 | CVPR | RGB drone | City block (~1 km²) | 20.93–24.06 | 0.547–0.575 | Photometric only | Mill-19 (Building, Rubble) | yes |
| Sat-NeRF [B1] | 2022 | CVPR Workshops (EarthVision) | WorldView-3 satellite | Single-city block (256×256 m) | 24.80–26.16 | 0.876–0.951 | DSM altitude MAE 1.3–2.4 m | DFC2019 / GRSS Jacksonville (JAX) | yes |
| VastGaussian | 2024 | CVPR | RGB drone | Multi-block (~1–2 km²) | 23.50–26.92 | 0.804–0.885 | Photometric only | Mill-19, UrbanScene3D | yes |
| Aira et al. (EOGS) [8] | 2025 | CVPR | WorldView-3 satellite (RPC) | Single-city block (256×256 m) | n/a (photometric loss only reported) | n/a | DSM elevation MAE 1.46 m (JAX mean); MAE 1.62 m (IARPA mean) | DFC2019 / IARPA MVS3DM | yes |
| Gao et al. [9] | 2025 | IEEE TGRS | Google Earth imagery (oblique) | City scale (~165 km²) | 27.0–30.7 | 0.851–0.964 | Photometric only (point-cloud densification reported qualitatively) | BungeeNeRF cities (11 scenes: New York, Waterloo, etc.) | no |
| Sun et al. [14] | 2025 | Comput. Graph. Forum | RGB aerial (ultra-high-res) | Large aerial block | n/a | n/a | Photometric only | Proprietary ultra-high-resolution aerial dataset | no |
| Mei et al. [12] | 2025 | IEEE Access | UAV RGB (low-altitude) | Large UAV scene | n/a | n/a | Photometric only | Proprietary low-altitude UAV dataset | no |
| Octree-GS [33] | 2025 | IEEE TPAMI | RGB camera | City block (multi-scale LoD) | 26.41–27.14 | 0.814–0.829 | Photometric only | MatrixCity (Block_All), Mip-NeRF 360 | yes |
| CityGaussian | 2024 | ECCV | RGB aerial / street | City scale (2.7 km² small city) | 27.46 (MatrixCity small city) | n/a | Photometric only | MatrixCity | yes |
| ARSGaussian / RSGaussian [17] | 2026 | ISPRS J. Photogramm. Remote Sens. | Aerial RGB + LiDAR | Aerial block (~1 km²) | 26.75–26.91 | 0.858–0.876 | LiDAR RMSE 0.14–0.28 m | UR3D (Artsci), AIR-LONGYAN | partial |
| LI-GS [43] | 2025 | IEEE Robot. Autom. Lett. | RGB camera + 3D LiDAR | Large outdoor (~1 km) | n/a | n/a | 52.6% improvement over LiDAR-only; 68.7% over GS-only (Chamfer distance) | Proprietary large-scale outdoor scenes | no |
| LIV-GaussMap [41] | 2024 | IEEE Robot. Autom. Lett. | LiDAR + IMU + camera | Indoor–outdoor (unbounded) | 30.17–31.84 (interpolated, indoor) | n/a | Chamfer distance + EMD reported | HKUST indoor / outdoor LIV dataset | yes |
| SAR-GS [156] | 2025 | arXiv 2506.21633 | Synthetic Aperture Radar (SAR) | Vehicle-target scale | Outperforms SAR-NeRF baseline (exact dB n/a in preprint) | Outperforms SAR-NeRF baseline | Chamfer distance + F1-score on MSTAR dataset | Rendered SAR dataset (T72, BTR80, KRAZ); MSTAR (real) | no |

### Notes on Table 2 entries

- **3DGS [6]:** PSNR 27.21 / SSIM 0.815 are the canonical Mip-NeRF 360 single-scale test values reported in the Mip-Splatting paper [A5] Table 4 (retrained baseline); the original 3DGS paper reports 27.21 / 0.815 on the same protocol. Tanks and Temples Train scene: PSNR ≈ 22.01 / SSIM 0.813 (Octree-GS supplementary).
- **Mega-NeRF [B4]:** Mill-19 Building PSNR 20.93, SSIM 0.547; Rubble PSNR 24.06, SSIM 0.553 (Table 2 of original paper, run to completion).
- **Sat-NeRF [B1]:** JAX 068 test view PSNR 24.80 / SSIM 0.903; JAX 214 PSNR 25.54 / SSIM 0.951 (best single-AOI results, row 4 of original paper Table 1); altitude MAE range 1.28–2.43 m across four JAX AOIs.
- **VastGaussian:** Building PSNR 23.50 / SSIM 0.804; Rubble PSNR 26.92 / SSIM 0.823; Residence PSNR 24.25 / SSIM 0.852 (Table 1 of CVPR 2024 paper).
- **Aira et al. EOGS [8]:** The paper focuses on geometric accuracy (DSM elevation MAE) rather than photometric metrics; PSNR/SSIM for the satellite-adapted 3DGS pipeline are not explicitly tabulated and are therefore listed as n/a.
- **Gao et al. [9]:** Test PSNR range 27.0–30.7 across 11 Google Earth city scenes; SSIM range 0.851–0.964; best single scene (New York) PSNR 30.7 / SSIM 0.964.
- **Octree-GS [33]:** MatrixCity Block_All PSNR 26.41 / SSIM 0.814 (github checkpoints); Mip-NeRF 360 Block_Small PSNR 27.14 / SSIM 0.829 (TPAMI paper, Table 3).
- **ARSGaussian [17]:** UR3D(Artsci) PSNR 26.75 / SSIM 0.876, LiDAR RMSE 0.283 m; AIR-LONGYAN PSNR 26.91 / SSIM 0.858, LiDAR RMSE 0.137 m (Table 1 of arXiv 2412.18380).
- **LIV-GaussMap [41]:** PSNR values are for indoor interpolated views; outdoor extrapolation degrades significantly (PSNR 15–24 dB), reflecting the inherent difficulty of unbounded scenes.
- **SAR-GS [156]:** arXiv 2506.21633; exact PSNR/SSIM dB values are stated to surpass SAR-NeRF but are presented in a figure rather than a table in the preprint; exact numbers not extractable.

---

**Table 2 Caption.** This table collates representative methods spanning the full spectrum from general-purpose 3D Gaussian Splatting to domain-adapted pipelines for satellite, aerial UAV, LiDAR-fused, and SAR imaging. Several key trade-offs emerge. Methods reporting only photometric metrics (PSNR/SSIM) — including vanilla 3DGS [6], Mip-Splatting [A5], CityGaussian, and Octree-GS [33] — optimise rendering fidelity but cannot certify sub-metre spatial accuracy required by mapping or inspection workflows. Conversely, Aira et al. (EOGS) [8], Sat-NeRF [B1], and ARSGaussian [17] explicitly report geometric accuracy (DSM elevation MAE, LiDAR RMSE), often at the cost of lower photometric scores, reflecting the fundamental photometric-vs-geometric trade-off that motivates the five-dimension evaluation framework in §5. Regarding dataset scope: Mip-NeRF 360 and Tanks and Temples are indoor/bounded-outdoor benchmarks designed for close-range NVS, while Mill-19, UrbanScene3D, and MatrixCity represent city-block-scale outdoor scenarios. DFC2019/IARPA MVS3DM and the AIR-LONGYAN dataset are the primary satellite and aerial-LiDAR benchmarks, respectively. The Oxford Spires dataset [15] additionally provides millimetre-accurate TLS ground truth for outdoor localisation and reconstruction benchmarking. The absence of entries in the Geometric accuracy column for most camera-only methods highlights a critical gap: photometric metrics alone are insufficient proxies for the GD&T compliance requirements encountered in aerospace and infrastructure inspection applications.

---

## Table 3: 3DGS-based Industrial and Infrastructure Digital-Twin Works

| Work | Year | Application domain | Sensors | Scene type | Dynamic? | Reported metrics | Deployment status |
|---|---|---|---|---|---|---|---|
| Rebolj et al. (Scan-vs-BIM) [I1] | 2017 | AEC / construction progress monitoring (pre-3DGS baseline) | TLS point cloud vs BIM model | Building construction site | No | Point-cloud-to-BIM geometric tolerance (±6–10 mm threshold for structural elements) | Open dataset; methodology standard |
| Sheikh (BIM-based 4D reconstruction) [I2] | 2024 | AEC / construction 4D digital twin | RGB video + BIM model | Multi-storey building construction | Yes (construction sequence) | IFC alignment RMSE; schedule deviation detection | PhD dissertation; lab demonstration |
| PerfCam [22] | 2025 | Smart manufacturing / production-line monitoring | RGB camera + IoT sensors (vibration, force, temperature) | Pharmaceutical conveyor-belt production line | Yes (conveyor belt, moving products) | OEE extraction accuracy (product count near-100% per-frame accuracy); PSNR/SSIM of 3DGS reconstruction not reported separately | Production pilot (AstraZeneca test line); open dataset |
| Cui et al. LetsGo [21] | 2024 | Smart facility / multi-storey garage digital twin | LiDAR (handheld) + RGB camera | Large-scale indoor garage (GarageWorld) + KITTI-360 outdoor | No (static scene) | PSNR 25.77, SSIM 0.812 (GarageWorld); PSNR 24.53, SSIM 0.811 (KITTI-360) | Open dataset; lab demonstration |
| Hong et al. LIV-GaussMap [41] | 2024 | Mobile robotics / real-time mapping for DT | LiDAR (Ouster OS1-128, Livox Avia, RealSense L515) + IMU + camera | Indoor and outdoor large-scale scenes (multi-sensor) | No (static mapping) | PSNR 30.17–31.84 (indoor interpolated); Chamfer distance + EMD for structure | Open dataset; lab demonstration |
| Hong et al. GS-LIVO [42] | 2025 | LiDAR-inertial-visual SLAM for DT mapping | LiDAR + IMU + camera | Indoor garage, outdoor island, airport scenes | No (static scenes, real-time mapping) | PSNR 25.34–27.52 (indoor); real-time mapping at >10 Hz indoor / ~3 Hz outdoor | Lab demonstration; open-source |
| Yang et al. MFGaussian [49] | 2025 | Multi-modal scene representation for DT | Mobile Laser Scanner (MLS) + camera | Indoor and outdoor mixed scenes | No | Outperforms 3DGS, NeRF, and Mip-Splatting on proprietary dataset + ETH3D stereo; exact dB n/a in preprint | Open dataset planned; lab demonstration |
| Wang et al. ROS-based online 3DGS [24] | 2025 | Robotics / real-time DT update | RGB-D camera / any ROS-compatible sensor | Indoor / outdoor robotic scenes | No (online reconstruction) | PSNR comparable to offline 3DGS; latency metrics reported | Lab demonstration; open-source ROS package |

### Notes on Table 3 entries

- **Rebolj et al. [I1]:** *Automation in Construction* 84 (2017). This is a pre-3DGS photogrammetric baseline establishing point-cloud-to-BIM geometric fidelity thresholds that remain the de-facto acceptance criteria (±6 mm for structural steel, ±10 mm for concrete) against which 3DGS-based inspection workflows should be benchmarked (see §5 criterion C4).
- **Sheikh [I2]:** PhD dissertation, Ghent University (2024). Demonstrates BIM-integrated 4D reconstruction covering construction sequence monitoring; provides a comprehensive framing of the AEC digital-twin use case for §6.6.
- **PerfCam [22]:** arXiv 2504.18165 / IEEE Access 2025. The 3DGS component is used for static scene modelling of the production line (2002 RGB frames, 26 camera positions); dynamic KPI extraction relies on YOLOv11 object detection layered on top of the static twin. Photometric reconstruction quality (PSNR/SSIM) of the 3DGS component is not separately tabulated — the paper reports task-level KPIs (OEE, availability, throughput counts) rather than rendering metrics.
- **LetsGo [21]:** ACM TOG / SIGGRAPH Asia 2024. Uses a custom polar-coordinate handheld scanner. LOD-LiDAR-GS achieves best results among all compared methods on GarageWorld and KITTI-360; geometry-only LiDAR initialisation without visual optimisation ("Case II" ablation) shows that LiDAR alone degrades PSNR in complex scenes.
- **LIV-GaussMap [41]:** IEEE Robot. Autom. Lett. 2024. Reports both photometric (PSNR, interpolated vs extrapolated views) and structural (Chamfer distance, EMD) metrics; notably, using LiDAR initialisation without photometric refinement can reduce PSNR in complex outdoor scenes, illustrating that sensor fusion must be carefully balanced.
- **GS-LIVO [42]:** IEEE Trans. Robot. 2025. The first real-time Gaussian-based SLAM system deployable on an embedded platform (NVIDIA Jetson Orin NX); achieves >10 Hz mapping update indoors and ~3 Hz outdoors, establishing a practical throughput benchmark for edge-deployed digital twin systems.
- **MFGaussian [49]:** Int. J. Digit. Earth 2025. Employs a stepwise training strategy (pre-train on virtual views from colour point cloud, then fine-tune on real views) to handle sparse inputs from MLS without SfM; directly relevant to factory-floor scenarios where sensor coverage is incomplete.
- **Wang et al. [24]:** Sensors 2025. Focuses on the engineering integration layer (ROS frontend + online 3DGS backend) rather than reconstruction quality per se; establishes the software-architecture precedent for plug-and-play DT deployment in robotic workcells.

---

**Table 3 Caption.** The industrial and infrastructure digital-twin literature surveyed in this table exhibits a reporting style markedly different from the remote-sensing benchmark culture of Table 2. Works targeting production monitoring and construction progress (PerfCam [22]; Rebolj et al. [I1]; Sheikh [I2]) focus on task-level KPIs — OEE, schedule deviation, and scan-to-BIM tolerances — rather than photometric metrics such as PSNR or SSIM. In contrast, robotics-oriented mapping systems (LIV-GaussMap [41]; GS-LIVO [42]; LetsGo [21]) do report PSNR but additionally include structural accuracy metrics (Chamfer distance, EMD) that are more relevant to inspection tasks. This bifurcation reflects a fundamental tension in the field: photometric metrics measure visual plausibility, while task-level KPIs and geometric tolerances measure operational utility. For aerospace and AEC digital twins, the latter are the decision-relevant criteria, motivating the GD&T-grounded evaluation framework proposed in §5 of this review.

---

*End of Tables 2 and 3.*

