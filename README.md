# Mango Leaf AI Diagnosis

**Mango Leaf AI Diagnosis** is an AI-driven application designed to automatically detect and classify diseases in mango leaves using image analysis and machine learning/deep learning models. This project aims to assist farmers and agricultural professionals by providing quick and accurate leaf health diagnostics and actionable insights.
The system leverages computer vision techniques and trained models to identify diseases such as anthracnose, powdery mildew, bacterial canker, and more from leaf images.

---
Plant diseases can significantly reduce crop yields if not detected early. Manual inspection is time-consuming and error-prone. This repository provides an **AI/ML model pipeline** to classify mango leaf diseases automatically using image data. Models are trained on labeled leaf images and integrated into an application interface for end-user use.

---

## Features

* Image upload and disease diagnosis
* Trained using convolutional neural networks (CNN) or transfer-learning models
* Multi-class classification for multiple mango leaf diseases

---
### Prerequisites

Before running the project, ensure the following are installed:

* Python 3.8+
* pip (Python package manager)
* Virtual environment (recommended)


## Dataset
The dataset contains mango leaf images labeled with their respective disease categories. The images should be organized by folder for each class such as:

```
│── dataset/
    ├── Healthy/
    ├── Anthracnose/
    ├── Powdery_Mildew/
    ├── Bacterial_Canker/
```


## Model Training

1. Load and preprocess images
2. Split dataset into training and validation sets
3. Load pretrained CNN Model (VGG16) -> Pretrained on ImageNet-> Uses small 3×3 filters ->Fine-tuned for mango leaf disease detection
4. Train model
5. Evaluate accuracy
---

## Results
86% with VGG-16 Cnn 
---
## Contribution

Contributions, issues, and feature requests are welcome.
Feel free to open an issue or submit a pull request.

---

## License

This project is licensed under the **MIT License**.

[1]: https://data.mendeley.com/datasets/j3bn63t4sp/2?utm_source=chatgpt.com "Mango Leaf Disease Detection Dataset Using Deep Learning"
[2]: https://github.com/IsaacMwendwa/Omdena-Mango-Leaf-Disease-Detection?utm_source=chatgpt.com "IsaacMwendwa/Omdena-Mango-Leaf-Disease-Detection - GitHub"
