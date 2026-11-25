[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/brain-life/abcd-spec)
[![Run on Brainlife.io](https://img.shields.io/badge/Brainlife-bl.app.313-blue.svg)](https://doi.org/10.25663/brainlife.app.313)

### Author
- Hanna Willis (hanna.willis@ndcn.ox.ac.uk)

# app-combine-roi-scans

<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

> **Copies a set of ROIs together with a preprocessed DWI and a T1-weighted image into one folder for visual checking.**

A small utility (adapted from svincibo/app-combineROI) that copies every ROI file, the DWI and the T1w image into output/rois so they can be viewed together. It does no image processing or resampling.

| | |
|---|---|
| 📥 **Inputs** | `neuro/rois` · `neuro/dwi` · `neuro/anat/t1w` |
| 📤 **Outputs** | `raw` |
| ⚙️ **Resources** | 1 CPUs |
| 🔗 **Run it** | [doi.org/10.25663/brainlife.app.681](https://doi.org/10.25663/brainlife.app.681) |

#### 📥 Inputs

| Input | Datatype | Required | Description |
|---|---|---|---|
| `rois` | `neuro/rois` | yes | ROI volumes to include. |
| `dwi` | `neuro/dwi` (preprocessed) | yes | Preprocessed DWI to include. |
| `anat` | `neuro/anat/t1w` (preprocessed) | yes | Preprocessed T1-weighted image to include. |

#### 📤 Outputs

| Output | Datatype | Description |
|---|---|---|
| `output` | `raw` | Folder containing the ROIs, the DWI and the T1w image for visual checking. |

<!-- brainlife-app:end -->

This app will combine multiple ROI datatypes, diffusion scans and t1 scans into one ROI file. 
This app is adapted from svincibo/app-combineROI.
