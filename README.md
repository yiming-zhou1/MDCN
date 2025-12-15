# MDCN
This is the code for our paper `Multi-angle Joint Distance Network for Combinatorial Medication Recommendation`.

For replication of the drug recommendation outcomes reported in this paper, please refer to the guidelines below.

# Overview

We have modularized and encapsulated the code to enhance its readability and maintainability. In summary, the MDCN can be split into two core components: the feature extractor and the prediction head. The feature extractor primarily captures multi-dimensional clinical feature representations of patients, while the prediction head computes the classification probability for each medical condition label.


# Requirements
Ensure your local environment meets the following requirements before installation:

| Package          | Version Requirement |
|------------------|---------------------|
| PyTorch          | 1.9 ≤ version ≤ 1.12.1 |
| NumPy            | == 1.15.1           |
| Python           | ≥ 3.8               |
| scikit-learn     | ≥ 0.24.2            |

> ⚠️ Note: PyTorch version is constrained to 1.9 ~ 1.12.1 (inclusive) for compatibility with core modules. We recommend installing PyTorch with CUDA support if GPU acceleration is available (see [PyTorch Official Installation Guide](https://pytorch.org/get-started/previous-versions/) for version-specific commands).


# Dataset
We provide the dataset in the `data/` folder. 
The experimental data in this project is derived from the **MIMIC-III** (Medical Information Mart for Intensive Care III) and **MIMIC-IV** datasets — two large-scale public clinical databases containing de-identified intensive care unit (ICU) patient records. For complete raw data (including full clinical notes, lab results, and prescription records), please refer to the official MIMIC repositories:
- MIMIC-III: [PhysioNet/MIMIC-III Clinical Database](https://physionet.org/content/mimic3/1.4/)
- MIMIC-IV: [PhysioNet/MIMIC-IV Clinical Database](https://physionet.org/content/mimiciv/2.2/)
