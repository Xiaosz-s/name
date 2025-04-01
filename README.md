<div align="center">
<h1> Reconsidering Parking Slot Detection: Robust, Scalable, User-Friendly
and End-to-End Framework </h1>

[Zhenjie Duan](), [Yaoming Zhuang](), [Yifan Chao]() , [Pengcheng Zhu](),[Li Li](), [Chengdong Wu](), [Zhanlin Liu]()

 ---
## Introduction
<div align="center"><h4><!-- Project Short Description or Slogan --></h4></div>

![framework](/media/framework.png "framework")

Accurate parking slot detection is crucial for
autonomous valet parking and intelligent driving, directly
impacting safety and efficiency. However, most existing methods
rely on VAM images, making them susceptible to image distortion and vehicle occlusion. Additionally, many approaches
independently regress corner points without considering the
overall parking slot structure, limiting detection accuracy and
necessitating post-processing. To address these challenges, we
propose BEV-PolyNet, a novel end-to-end detection framework.
By leveraging surround-view images to generate BEV feature,
our method mitigates distortion and occlusion issues. We
introduce a polygonal modeling approach that preserves the
integrity of parking slots while accommodating complex shapes.
Furthermore, we enhance detection accuracy and convergence
speed by initializing query vectors with features from surroundview monitoring images, combined with location prior encoding.
Extensive experiments on the public PS2.0 dataset and a private
LPD dataset validate the effectiveness of BEV-PolyNet, demonstrating its superior performance in parking slot detection.

---

## 🎥 Demonstration Video

https://github.com/user-attachments/assets/a85dd69e-3b2c-44a9-8012-6ef3f509f9d6

---

## Dataset
We restructured the datasets. For the **PS2.0 dataset**, we converted the original `.mat` format to `.pkl`. For the **PIL-Park Dataset**, we used data with parking spaces fully visible in the images, selecting the relevant data and converting the `.txt` labels to `.pkl` format.

### 📁 PS2.0 Dataset Usage Instructions

The `.pkl` file contains `keypoint_results` for each parking space entrance line with two keypoints.

[Download PS2.0 Dataset](https://drive.google.com/file/d/1zR3kmKvUZg0l85NDVan_JVF_bEnaepPw/view?usp=sharing)

### 📁 PIL-Park Dataset Usage Instructions

The `.pkl` file contains `keypoint_results` for each parking space with four keypoints and a center point.

[Download PIL-Park Dataset](https://drive.google.com/file/d/1Ux4blvcuS9cxg3133NzYC1tekupLc44m/view?usp=sharing)

---

