---
layout: page
title: ""
path: "/catalyst/"
---

## CATALYST: An R-based reproducible and user-friendly preprocessing pipeline for CyTOF data

Helena L. Crowell<sup>1</sup>, Stéphane Chevrier<sup>1</sup>, Andrea Jacobs, Sujana Sivapatham, Tumor Profiler Consortium, Bernd Bodenmiller<sup>1</sup>, Mark D. Robinson<sup>1</sup>

<sup>1</sup>_Equal contribution_<br/>

### Abstract

Mass cytometry (CyTOF) has become a method of choice for in-depth characterization of tissue heterogeneity in health and disease, and is currently implemented in multiple clinical trials, where higher quality standards must be met. Currently, preprocessing of raw files is commonly performed in independent standalone tools, which makes it difficult to reproduce. Here, we present an R pipeline based on an updated version of CATALYST that covers all preprocessing steps required for downstream mass cytometry analysis in a fully reproducible way. This new version of CATALYST is based on Bioconductor’s SingleCellExperiment class and fully unit tested. The R-based pipeline includes file concatenation, bead-based normalization, single-cell deconvolution, spillover compensation and live cell gating after debris and doublet removal. Importantly, this pipeline also includes different quality checks to assess machine sensitivity and staining performance while allowing also for batch correction. This pipeline is based on open source R packages and can be easily be adapted to different study designs. It therefore has the potential to significantly facilitate the work of CyTOF users while increasing the quality and reproducibility of data generated with this technology.

### Software availability

Analyses in the publication were run in R v4.0.036, with Bioconductor v3.1137, and all software packages used throughout this workflow are publicly available through the [Comprehensive R Archive Network](https://cran.r-project.org) or the [Bioconductor project](http://bioconductor.org).

### Publications

- [F1000Research](https://f1000research.com/articles/9-1263), October 2020.

### Data

* [CyTOF_acquisition_1-3.FCS](https://tpreports.nexus.ethz.ch/download/catalyst/data/CyTOF_acquisition_1-3.FCS.zip)
* [spillover_matrix.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/spillover_matrix.csv)
* [ref_bead_counts.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/ref_bead_counts.csv)
* [debarcoding_scheme.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/debarcoding_scheme.csv)
* [ref_marker_levels.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/ref_marker_levels.csv)
* [ref_cell_counts.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/ref_cell_counts.csv)
* [normalization_beads.fcs](https://tpreports.nexus.ethz.ch/download/catalyst/data/normalization_beads.fcs)
* [sample_cell_counts.csv](https://tpreports.nexus.ethz.ch/download/catalyst/data/sample_cell_counts.csv)

* [All files (.tar, 297MB)](https://tpreports.nexus.ethz.ch/download/catalyst/data/catalyst_data.tar)