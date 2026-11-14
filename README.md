# 🌿 Plant Disease Detection Using Deep Learning

## Overview

This project presents a deep learning-based plant disease detection system that identifies diseases from leaf images. The model is trained using a convolutional neural network (MobileNetV2) through transfer learning to achieve high accuracy while remaining lightweight for edge deployment.

## Features

* Detects multiple plant diseases from leaf images
* Transfer learning using MobileNetV2
* High classification accuracy
* TensorFlow Lite (TFLite) export for embedded devices
* Suitable for deployment on ESP32, Raspberry Pi, and other edge AI platforms

## Dataset

* **Source:** Custom Plant Disease Dataset
* **Total Images:** 9,000+
* **Classes:** 9

Example classes:

* Healthy
* Early Blight
* Late Blight
* Leaf Mold
* Bacterial Spot
* Mosaic Virus
* Powdery Mildew
* Rust
* Leaf Curl

## Model

* Architecture: MobileNetV2
* Framework: TensorFlow / Keras
* Image Size: 160 × 160
* Loss Function: Categorical Crossentropy
* Optimizer: Adam

## Project Structure

```text
Plant-Disease-Detection/
│
├── dataset/
├── notebooks/
├── model/
│   ├── plant_disease_model.h5
│   └── plant_disease_model.tflite
├── labels.txt
├── inference.py
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Plant-Disease-Detection.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## Training

Train the model using TensorFlow/Keras.

Example:

```python
python train.py
```

## Inference

Run prediction on a leaf image:

```python
python inference.py --image leaf.jpg
```

Example output:

```text
Prediction : Early Blight
Confidence : 98.42%
```

## Deployment

The trained model can be exported as:

* TensorFlow Lite (.tflite)
* Arduino Library
* Edge AI compatible model

Supported devices include:

* ESP32
* ESP32-CAM
* Raspberry Pi
* NVIDIA Jetson
* Other TensorFlow Lite-compatible edge devices

## Performance

| Metric              |       Value |
| ------------------- | ----------: |
| Training Accuracy   |        98%+ |
| Validation Accuracy |        95%+ |
| Framework           |  TensorFlow |
| Model               | MobileNetV2 |

*Performance depends on the dataset and training configuration.*

## Requirements

* Python 3.10+
* TensorFlow
* NumPy
* OpenCV
* Matplotlib
* Pillow

Install dependencies:

```bash
pip install tensorflow numpy opencv-python matplotlib pillow
```

## Future Improvements

* Real-time disease detection
* Explainable AI (Grad-CAM)
* Mobile application integration
* Edge AI optimization
* Multi-crop disease detection

## Author

**Ramanathan PL**

Pre-Final Year, Electronics and Communication Engineering (ECE)

PSNA College of Engineering and Technology

## License

This project is released under the MIT License.
