# P01 Perplexity Exchange Package

This is a public, sanitized exchange package for the P01 review manuscript:

**3D Gaussian Splatting for Remote Sensing and Aviation Digital Twins: A Review**

Target journal: **ISPRS Journal of Photogrammetry and Remote Sensing**

## Purpose

This repository is a controlled public bridge for external AI-assisted review and literature checking. It is not the full internal project workspace.

Use this repository to:

- review the current manuscript draft;
- check references and missing literature;
- improve wording, structure, and reviewer-facing argumentation;
- suggest figure/table revisions;
- return proposed changes as Markdown patches or clearly separated replacement sections.

## Contents

- `manuscript/`: current manuscript draft and revision log
- `figures/`: selected public figure/table materials for review
- `references/`: reference list and verification materials
- `tasks/`: task prompts for Perplexity or other external research tools
- `incoming_suggestions/`: place returned suggestions or patch-style outputs here before merging internally

## Important Boundary

The official working repository remains the internal Gitea repository. This public repository is only an exchange layer.

Do not add internal planning files, credentials, local paths, private meeting notes, student handoff packages, or unapproved source data here.

## Preferred Return Format

External tools should return one of the following:

1. A section-by-section Markdown revision proposal.
2. A patch-style file under `incoming_suggestions/`.
3. A structured review report with exact file names and section headings.

Final integration should be done in the internal P01 repository after human review.
