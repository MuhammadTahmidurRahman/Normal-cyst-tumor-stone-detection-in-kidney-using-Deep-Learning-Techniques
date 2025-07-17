# KidNet: Kidney Disease Classification in CT Images

**KidNet** is a TensorFlow/Keras pipeline for classifying kidney conditions—normal, cyst, stone, tumor—from abdominal CT scan slices.

## 🚀 Features

- Watershed-based ROI extraction & resizing
- Data augmentation (rotation, flip, brightness, etc.)
- Custom 18-layer CNN plus benchmarks (VGG16, ResNet50, MobileNetV2, EfficientNetB0, InceptionV3)
- Stratified train/val/test split (70/15/15)
- Metrics & visualizations: accuracy, loss, AUC, confusion matrices, ROC curves, sample predictions

## 📂 Repository Structure

```
kidney-classification/
├── data/                   # Unzipped ct-kidney/ dataset
│   ├── normal/
│   ├── cyst/
│   ├── stone/
│   └── tumor/
├── Kidney (1).ipynb        # Main notebook with preprocessing, training, and evaluation
├── cse465 Final Report.pdf # Written report detailing methodology and results
├── requirements.txt        # Python dependencies
├── LICENSE                 # MIT license
└── README.md               # This file
```

## ⚙️ Prerequisites

- Python ≥ 3.8
- pip

## 🛠 Installation

```bash
git clone https://github.com/your-username/kidney-classification.git
cd kidney-classification
pip install -r requirements.txt
```

## ▶️ Usage

1. Download the **CT KIDNEY** dataset from Kaggle and unzip into the `data/` folder.
2. Open and run the notebook:
   ```bash
   jupyter notebook "Kidney (1).ipynb"
   ```
3. Execute all cells to preprocess data, train models, evaluate performance, and generate visualizations.

## 📈 Sample Results

- **18-layer CNN:** 100% test accuracy, AUC = 1.00
- **InceptionV3:** 100% test accuracy, AUC = 1.00
- **MobileNetV2 / EfficientNetB0:** >99.5% accuracy
- **ResNet50:** Slight overfitting observed (see report)

## 📄 License

This project is released under the MIT License. See the `LICENSE` file for details.

## 🙏 Acknowledgements

- **Kaggle CT KIDNEY** dataset creators
- TensorFlow & Keras communities
- CSE465 course instructors for guidance

