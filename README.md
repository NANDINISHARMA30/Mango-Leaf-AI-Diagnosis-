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
* Live feedback with confidence scores
* Web interface or API for integration

---

## Getting Started

### Prerequisites

Before running the project, ensure the following are installed:

* Python 3.8+
* pip (Python package manager)
* Virtual environment (recommended)

---

### Installation

1. Clone the repository:

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/Mango-Leaf-AI-Diagnosis.git
cd Mango-Leaf-AI-Diagnosis
```

2. Create and activate a virtual environment (optional but recommended):

**Windows:**

```bash
python -m venv venv
.\venv\Scripts\activate
```

**Mac/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install required packages:

```bash
pip install -r requirements.txt
```

---

### Running the Application

#### Option A — Web Interface (Streamlit)

If your project contains a Streamlit app:

```bash
streamlit run app.py
```

Open the browser at:

```
http://localhost:8501
```

#### Option B — API Backend

If your project has a FastAPI or Flask backend:

**FastAPI example:**

```bash
uvicorn main:app --reload
```

**Flask example:**

```bash
python main.py
```

---

## Dataset

The dataset contains mango leaf images labeled with their respective disease categories. The images should be organized by folder for each class such as:

```
│── dataset/
    ├── Healthy/
    ├── Anthracnose/
    ├── Powdery_Mildew/
    ├── Bacterial_Canker/
```

You can use public datasets such as MangoLeafBD from Mendeley or custom collected leaf images. ([Mendeley Data][1])

---

## Model Training

1. Load and preprocess images
2. Split dataset into training and validation sets
3. Load pretrained CNN (e.g., ResNet50, MobileNet)
4. Train model
5. Evaluate accuracy
6. Save model weights for inference

---

## Usage

After starting the app or API:

1. Upload a mango leaf image
2. The system will display:

   * Predicted class (e.g., Anthracnose)
   * Confidence score
3. View recommended actions or treatments (if implemented)

---

## Project Structure

```
Mango-Leaf-AI-Diagnosis/
├── dataset/                  # Images for training and testing
├── app/                     # Frontend app (Streamlit/Flask)
├── models/                  # Saved trained models
├── notebooks/               # Training and EDA notebooks
├── src/                     # Code for training and inference
├── requirements.txt
└── README.md
```

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
