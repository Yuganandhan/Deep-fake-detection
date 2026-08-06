
# 🕵️ Deepfake Detection using Ensemble Learning

A deep learning-based Deepfake Detection system that identifies whether a face image is **Real** or **Fake** using an ensemble of **MobileNetV2** and **EfficientNetV2B0**. The project also includes **Grad-CAM visualization** for model interpretability and a **Gradio web application** for easy interaction.

---

## 📌 Overview

Deepfakes generated using AI have become increasingly realistic, creating challenges in media authenticity and cybersecurity. This project addresses the problem by combining two powerful pretrained CNN models into an ensemble for improved detection performance.

The application accepts a face image as input and predicts whether it is genuine or manipulated, along with the prediction confidence and visual explanation using Grad-CAM.

---

## ✨ Features

- Deepfake image classification (Real/Fake)
- Ensemble model using MobileNetV2 and EfficientNetV2B0
- Transfer Learning with pretrained ImageNet weights
- Grad-CAM visualization for explainable AI
- Confidence score for predictions
- Interactive Gradio web interface
- Prediction logging support

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- MobileNetV2
- EfficientNetV2B0
- OpenCV
- NumPy
- Matplotlib
- Gradio
- Google Colab

---

## 📂 Project Structure

```
Deepfake-Detection/
│
├── Backup_copy_for_the_final_project.ipynb
├── README.md
├── requirements.txt
├── models/
│   ├── MobileNetV2 Model
│   ├── EfficientNetV2B0 Model
│   └── Ensemble Model
├── prediction_logs.csv
└── images/
```

---

## ⚙️ Model Architecture

### MobileNetV2
- Pretrained on ImageNet
- Transfer Learning
- Global Average Pooling
- Dropout Layer
- Sigmoid Output

### EfficientNetV2B0
- Pretrained on ImageNet
- Transfer Learning
- Global Average Pooling
- Dense Output Layer

### Ensemble Model
The outputs from MobileNetV2 and EfficientNetV2B0 are combined to generate the final prediction, improving robustness and overall performance.

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/deepfake-detection.git
cd deepfake-detection
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

Launch the notebook or execute the Gradio application.

```bash
python app.py
```

or

Open

```
Backup_copy_for_the_final_project.ipynb
```

in Google Colab or Jupyter Notebook.

---

## 📷 How It Works

1. Upload a face image.
2. Image is resized to **224 × 224**.
3. Pixel values are normalized.
4. Image is passed through both MobileNetV2 and EfficientNetV2B0.
5. Ensemble model predicts whether the image is Real or Fake.
6. Prediction confidence is displayed.
7. Grad-CAM highlights the regions influencing the prediction.

---

## 📊 Output

Example output:

```
Prediction: Fake

Confidence: 97.84%
```

The application also generates Grad-CAM heatmaps to explain the model's decision.

---

## 📈 Future Improvements

- Video deepfake detection
- Face extraction from videos
- Real-time webcam detection
- Support for multiple deepfake datasets
- Model optimization for mobile deployment
- Improved ensemble strategies

---

## 👨‍💻 Author

**Your Name**

Final Year Project – Deepfake Detection using Deep Learning

---

## 📄 License

This project is intended for educational and research purposes.
