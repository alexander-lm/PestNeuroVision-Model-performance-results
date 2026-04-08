# PestNeuroVision: Agricultural Pest Detection with YOLO11s

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)

A fine-tuned **YOLO11s** object detection model for identifying agricultural pest species across 9 classes, including adult insects, larvae, and nymphs.

---

## 📋 Overview

This model was trained to detect and classify common agricultural pests from images, supporting early pest identification for crop protection. It was evaluated on a held-out test set of **135 images** containing **368 instances** across 9 pest categories.

> **Full details of the model evaluation:** [View training notebook on Colab](https://colab.research.google.com/drive/183x539AQ803xicrouAUfIuG8OOdY1PqD#scrollTo=yvjMKYMGJWSy)

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

This project is distributed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**.
Any modifications or derivative works must also be distributed under the same license, with the source code made publicly available.

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)