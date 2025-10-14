# AVRDB-AFIO Cleaned Artery/Vein Masks

### 📋 Overview

This repository provides **cleaned and standardized artery/vein segmentation masks** derived from the publicly available **AVRDB dataset**
(*AVRDB: Annotated dataset for vessel segmentation and calculation of arteriovenous ratio*).
The annotations were originally provided by the **Armed Forces Institute of Ophthalmology (AFIO)**.

The original masks contained non-binary pixel values and near-white or near-red artifacts, which caused difficulties in segmentation training.
I refined and remapped the masks using the following color convention:

| Label      | RGB Color   |
| ---------- | ----------- |
| Artery     | (255, 0, 0) |
| Vein       | (0, 0, 255) |
| Crossing   | (0, 255, 0) |
| Background | (0, 0, 0)   |

---

### 📁 Contents

* `/images`: RGB images
* `/av-labels`: processed artery/vein masks
* `samples/`: sample examples for illustration

---

### 📖 Citation Summary

#### Original Dataset

> Akbar, S., Hassan, T., Akram, M. U., Yasin, U. U., & Basit, I. (2017). AVRDB: Annotated Dataset for Vessel Segmentation and Calculation of Arteriovenous Ratio. In Proceedings of the International Conference on Imaging, Signal Processing and Pattern Recognition (IPCV'17), pp. 129-134.

#### This Work

```bibtex
@misc{trungdoavrdb,
  author       = {Thanh Trung Do},
  title        = {Cleaned and Standardized Artery/Vein Masks for the AVRDB Dataset},
  year         = {2025},
  howpublished = {\url{https://github.com/yourusername/AVRDB-AFIO-Cleaned-Masks}},
  note         = {Processed masks derived from AVRDB for segmentation research.}
}
```

---

### 📷 Samples

Below is an example image showcasing a few samples from the processed dataset (RGB image with overlayed masks):

![Sample Images](samples/sample_examples.png)

---

### 📧 Contact

For questions or access to the processing scripts, please contact:
📧 **[[trungdo1810.fw@gmail.com](mailto:trungdo1810.fw@gmail.com)]**

---

### ⭐ Support the Project

If you find this repository useful, please consider giving it a star ⭐ on GitHub! Your support helps motivate further improvements and sharing with the community.

---

### ⚠️ Ethical Note

This work aims to facilitate **reproducible research** in retinal artery/vein segmentation by providing cleaned versions of publicly available annotations.