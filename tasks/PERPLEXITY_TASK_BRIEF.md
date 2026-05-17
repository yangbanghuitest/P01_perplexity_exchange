# Perplexity Task Brief for P01

## Role

Act as a senior reviewer for ISPRS Journal of Photogrammetry and Remote Sensing. Focus on 3D Gaussian Splatting, remote sensing, aviation digital twins, airborne/spaceborne mapping, scene reconstruction, sensor fusion, geometry-aware evaluation, and reproducible review methodology.

## Main Files

- `manuscript/ISPRS_JPRS_Manuscript_v4_CN_20260514_working.md`
- `references/References_v3_Submission_Clean.md`
- `references/verified_references_30_cleaned.csv`
- `figures/Tables_2_3_v2.md`

## Tasks

1. Check whether the manuscript has a clear review scope for ISPRS JPRS.
2. Identify missing or weakly represented literature from 2023-2026, especially:
   - 3DGS and variants for large-scale outdoor scenes;
   - remote sensing, UAV, aerial mapping, satellite photogrammetry, and digital twins;
   - LiDAR/photogrammetry/NeRF/3DGS fusion;
   - geometry-aware metrics and uncertainty evaluation;
   - scene-level reconstruction under sparse views, scale variation, repetitive structures, and thin structures.
3. Suggest additions to the introduction and related-work framing.
4. Review whether the five-dimensional and nine-criterion evaluation framework is convincing.
5. Review Fig.7, Fig.8, and Fig.9 logic using the available figure/table materials.
6. Propose changes that make Section 6 a clear stress-test scenario rather than a competing paper theme.
7. Identify overclaiming, unsupported claims, and references that require verification.

## Output Format

Return the answer as a Markdown report with these sections:

- `Executive Summary`
- `Major Revision Suggestions`
- `Section-by-Section Edits`
- `Missing Literature Candidates`
- `Figure and Table Suggestions`
- `Reference Verification Risks`
- `Patch-Ready Text Blocks`

For each suggested literature item, include title, authors, year, venue, DOI or URL if available, and why it matters.

Do not ask for access to internal Gitea. Work only with this public exchange package.
