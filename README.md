# PestNeuroVision: A mobile application based on convolutional neural networks (CNNs) and computer vision for the detection of agricultural pests in the Cañete Valley, Lima, Peru

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)

This repository contains the performance evaluation results of the YOLO11s model conducted on the test dataset.

---

## 📋 Overview

The model was trained to detect and classify common agricultural pests from images, supporting early pest identification for crop protection. It was evaluated on a held-out test set of **135 images** containing **368 instances** across 9 pest classes.

> **Full details of the model evaluation:** [Link](https://github.com/alexander-lm/PestNeuroVision/blob/8da0490dd624244927c31acd7b47cebfcb35ec2e/colab-notebooks/03_Model_evaluation.ipynb)

---

### Overall Metrics

| Metric | Value |
|---|---|
| Precision | **0.924** |
| Recall | **0.877** |
| mAP@50 | **0.917** |
| mAP@50-95 | **0.780** |

### Per-Class Breakdown

| Class | Precision | Recall | mAP@50 | mAP@50-95 |
|---|---|---|---|---|
| *Bemisia tabaci* (adult) | 0.964 | 0.854 | 0.928 | 0.703 |
| *Ceratitis capitata* (adult) | 0.945 | 1.000 | 0.995 | 0.943 |
| *Dione juno* (adult) | 0.929 | 1.000 | 0.995 | 0.925 |
| *Dione juno* (larva) | 0.801 | 0.779 | 0.776 | 0.589 |
| *Ligyrus gibbosus* (adult) | 0.929 | 1.000 | 0.984 | 0.871 |
| *Liriomyza huidobrensis* (adult) | 1.000 | 0.910 | 0.960 | 0.858 |
| *Myzus persicae* (nymph) | 0.924 | 0.742 | 0.861 | 0.548 |
| *Spodoptera frugiperda* (adult) | 0.895 | 1.000 | 0.990 | 0.909 |
| *Spodoptera frugiperda* (larva) | 0.933 | 0.609 | 0.768 | 0.677 |

### Inference Speed (per image)

| Stage | Time (ms) |
|---|---|
| Preprocess | 4.8 |
| Inference | 9.4 |
| Postprocess | 3.5 |

---

## ⚖️ License

This project is licensed under the [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0).
The metrics and results presented here were generated using YOLO11 by Ultralytics, which is also governed by the [AGPL-3.0](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) license. All derivative works, including fine-tuned results and data, are distributed under these same terms. Any modifications or derivative works must also be distributed under the same license, with the source code made publicly available.

Full source code and license details are available in the [GitHub Repository](https://github.com/alexander-lm/PestNeuroVision).

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)