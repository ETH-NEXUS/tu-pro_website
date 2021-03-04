---
layout: page
title: ""
path: "/scim/"
---

## SCIM: Universal Single-Cell Matching with Unpaired Feature Sets

Stefan G. Stark<sup>1</sup>, Joanna Ficek<sup>1</sup>, Francesco Locatello, Ximena Bonilla, Stéphane Chevrier, Franziska Singer, Tumor Profiler Consortium, Gunnar Rätsch<sup>2</sup>, Kjong-Van Lehmann<sup>2</sup>
<sup>1</sup>_Equal contribution_<br/>
<sup>2</sup>_Correspondence to: Gunnar.Ratsch@ratschlab.org, Kjong.Lehmann@inf.ethz.ch_

### Motivation

Recent technological advances have led to an increase in the production and availability of single-cell data. The ability to integrate a set of multi-technology measurements would allow the identification of biologically or clinically meaningful observations through the unification of the perspectives afforded by each technology. In most cases, however, profiling technologies consume the used cells and thus pairwise correspondences between datasets are lost. Due to the sheer size single-cell datasets can acquire, scalable algorithms that are able to universally match single-cell measurements carried out in one cell to its corresponding sibling in another technology are needed.

### Results

We propose Single-Cell data Integration via Matching (SCIM), a scalable approach to recover such correspondences in two or more technologies. SCIM assumes that cells share a common (low-dimensional) underlying structure and that the underlying cell distribution is approximately constant across technologies. It constructs a technology-invariant latent space using an auto-encoder framework with an adversarial objective. Multi-modal datasets are integrated by pairing cells across technologies using a bipartite matching scheme that operates on the low-dimensional latent representations. We evaluate SCIM on a simulated cellular branching process and show that the cell-to-cell matches derived by SCIM reflect the same pseudotime on the simulated dataset. Moreover, we apply our method to two real-world scenarios, a melanoma tumor sample and a human bone marrow sample, where we pair cells from a scRNA dataset to their sibling cells in a CyTOF dataset achieving 93% and 84% cell-matching accuracy for each one of the samples respectively.

### Source code availability

[https://github.com/ratschlab/scim](https://github.com/ratschlab/scim)

### Publications

- [Bioinformatics](https://academic.oup.com/bioinformatics/article/36/Supplement_2/i919/6055906?login=true), September 2020.
- [bioRxiv](https://www.biorxiv.org/content/10.1101/2020.06.11.146845v3), June 2020.

### Open access data [[Manifest](https://tpreports.nexus.ethz.ch/download/scim/data/scim_manifest_md5sum.txt)]

- [PROSSTT simulated data](https://tpreports.nexus.ethz.ch/download/scim/data/prosstt/), Simulated datasets from three single-cell 'omics-styled technologies using PROSSTT (Papadopoulos et al., 2019).
- [Tumor Profiler data](https://tpreports.nexus.ethz.ch/download/scim/data/tupro/), Single-cell profile (CyTOF and scRNA-seq) of a metastatic melanoma sample from the Tumor Profiler Consortium