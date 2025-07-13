# 🚗 Blurred Image Object Detection

Image deblurring is a critical task in computer vision, especially for real-time systems like autonomous vehicles, surveillance cameras, medical imaging, and photography. These applications often face challenges due to motion blur, atmospheric interference, defocus, or optical distortions — caused by camera movement, object motion, or environmental conditions.

This project focuses on training object detection models that remain effective under such real-world blur conditions. A custom dataset of blurred images was manually annotated using Roboflow, and both YOLOv11 and YOLOv12 were benchmarked to evaluate detection performance in degraded visual scenarios.

---

## 📁 Dataset Overview

- **Size**: 1,000+ custom-annotated images
- **Annotation Tool**: [Roboflow Annotate](https://roboflow.com/annotate)


🗂️ **Dataset available on Roboflow Universe** 
<a href="https://universe.roboflow.com/image-deblurring/image-deblurring-ol1wo-bpcfn">
    <img src="https://app.roboflow.com/images/download-dataset-badge.svg"></img>
</a>
👉 [https://universe.roboflow.com/image-deblurring/image-deblurring-ol1wo-bpcfn]

---

## 🧠 Models & Results

We trained and evaluated two object detection models using the Ultralytics YOLO CLI:

| Model    | mAP@0.5 | Recall  | Precision |
|----------|---------|---------|-----------|
| YOLOv11  | 88.0%   | 81.9%   | 79.2%     |
| YOLOv12  | 87.3%   | 79.0%   | 80.8%     |

- **YOLOv11** achieved higher recall and overall performance on blurred objects  
- **YOLOv12** produced fewer false positives, with slightly better precision

---

## 🛠 Tools & Libraries

- Python 3.x  
- [Ultralytics YOLO CLI](https://docs.ultralytics.com)  
- OpenCV  
- Roboflow Annotate  
- Jupyter Notebook (for visualization and evaluation)


