# KT Neurovascular Screen

Computational candidate-screening workflow developed for the Klaus Tschira Boost Fund pre-proposal on sensory–vascular communication during pulmonary metastatic colonization.

## Purpose

This notebook performs a screen-first analysis to identify experimentally tractable ligand–receptor axes linking lung-innervating sensory neurons with pulmonary vascular/perivascular compartments and early metastatic responses.

The analysis is used for **candidate generation only**. The public datasets are independent experimental systems and do not establish animal-level causal relationships.

## Workflow

1. Download and cache public GEO datasets.
2. Build a pulmonary sensory-neuron signalling catalogue.
3. Construct ligand–receptor relationships using OmniPath and human-to-mouse orthology.
4. Quantify ligand expression across pulmonary sensory-neuron subtypes.
5. Evaluate receptor expression and vascular ageing effects.
6. Evaluate receptor/pathway responses during early B16F10 pulmonary metastatic seeding.
7. Incorporate pericyte and independent vascular datasets.
8. Rank candidate ligand–receptor axes using convergent evidence.
9. Export compact tables and figures for downstream experimental planning.

## Core datasets

- GSE186180 — pulmonary sensory-neuron Smart-seq2 atlas
- GSE124872 — young versus aged whole-lung single-cell RNA-seq
- GSE253749 — control, 6 h and 30 h B16F10 lung endothelial single-cell RNA-seq
- GSE137363 — lung pericyte-like cell RNA-seq
- GSE210291 — lung endothelial bulk RNA-seq
- GSE278974 — endothelial/fibroblast RNA-seq from B16F10 lung melanoma models

Additional validation datasets are handled within the notebook.

## Reproducibility

The notebook is designed for Google Colab and can also be run in a local Jupyter environment. Public input datasets are downloaded from their original repositories rather than stored in this repository.

The notebook records software versions and computes checksums for downloaded input files.

## Repository contents

- KT_neurovascular_screen_colab.ipynb — executable analysis workflow
- README.md — project and reproducibility documentation

No raw GEO datasets are redistributed here.

## Scientific scope

The analysis was developed to nominate sensory–vascular mechanisms for experimental testing. Candidate nomination should not be interpreted as evidence of coordinated regulation, signalling direction, or causality across the independent source datasets.
