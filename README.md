# AnchorHandoff: Anime Drag and Style Editing

This repository accompanies the paper:

**Coordinating Drag Based Structure Editing and Reference Style Transfer in Diffusion Models for Anime Images**

## Status

This repository is being organized for release. The implementation, evaluation scripts, configuration files, and benchmark annotation materials will be released upon publication.

At the current stage, this repository provides the project description, planned release contents, and data availability notes.

## Overview

AnchorHandoff is a temporally coordinated diffusion editing framework for joint anime drag and style editing. Given a content image, a style reference image, handle target points, and an edit mask, the method aims to perform local structure editing while transferring reference style to the edited layout.

The key idea is to separate drag optimization from style replay. Dragging is performed with style injection disabled, followed by a short interval for structure stabilization. A predicted clean sample is then used as an anchor for refreshing content queries and replaying reference style keys and values.

## Planned Release

The repository will include:

- Source code for AnchorHandoff
- Main experimental configuration files
- Annotation format for handle target points and masks
- Evaluation scripts for the metrics used in the paper
- Example cases and usage instructions
- Benchmark annotation materials where redistribution is permitted

## Data Notice

The original anime images used in the benchmark are sourced from publicly available datasets and are not redistributed because of source license restrictions.

Benchmark annotations and source records will be provided where redistribution is permitted. These materials are intended to support reproducibility without redistributing third party image data.

## Metrics

The planned evaluation scripts will cover the main metrics reported in the paper, including:

- Mean Distance
- Succ.@20
- Mask out IF
- ArtFID
- CFSD

## Citation

Citation information will be added after publication.

## Contact

For questions, please contact:

Youdong Ding  
ydding@shu.edu.cn
