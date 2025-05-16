
# DeepFake Detection Using Pre-Trained CNNs and Vision Transformers with Ensemble Learning

This repository contains the LaTeX source code and supplementary assets for a research project on detecting DeepFake images using various pre-trained deep learning models, including CNNs and Vision Transformers. The project investigates model performance, ensemble learning strategies, and architecture behaviors in data-constrained environments.

## 📄 Project Overview

DeepFakes pose a serious threat to digital media authenticity. This project evaluates the effectiveness of pre-trained Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs) on a subset of the FaceForensics++ dataset for binary classification of real vs. fake facial images. It explores the architectural benefits of each approach, especially under limited data conditions, and tests ensemble learning to enhance model robustness.

### Key Models Explored:
- **VGG16** (CNN baseline)
- **Vision Transformer (ViT)**
- **GenConViT** (Hybrid CNN-Transformer)
- **DeepFake-Adapter**

## 🧪 Methodology

- **Dataset:** 200-image subset from FaceForensics++ (100 real, 100 fake)
- **Image Size:** 128×128
- **Preprocessing:** Normalization, minimal augmentation
- **Training:** Fine-tuned using Binary Cross-Entropy loss, Adam optimizer, and early stopping
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score
- **Ensemble Learning:** Soft voting across multiple models

## 📊 Results

- **Best Accuracy:** 70% with VGG16
- **ViT Performance:** Underperformed due to data limitations
- **Ensemble Learning:** Minor improvement in prediction consistency

## 📁 Repository Structure

```

├── images/                         # All diagrams and figures used in the paper
│   ├── vgg16\_architecture.png
│   ├── vit\_architecture.png
│   ├── genconvit\_architecture.png
│   ├── deepfake\_adapter\_architecture.png
│   ├── sample\_faces.png
│   ├── confusion\_cnn.png
│   ├── confusion\_vit.png
│   ├── accuracy\_bar.png
│   └── metric\_comparison.png
│
├── DeepFake\_Detection.tex          # Main LaTeX source file
├── README.md                       # Project overview (this file)
└── references.bib (optional)       # BibTeX file for references (if separated)

```

## 🛠️ Dependencies

To compile the LaTeX document, ensure you have the following packages installed:
- `graphicx`
- `amsmath`
- `cite`
- `caption`
- `multirow`
- `booktabs`
- `hyperref`
- `placeins` (optional but recommended)

You can use a LaTeX distribution like **TeX Live**, **MiKTeX**, or an online editor like **Overleaf**.

## 📚 References

The paper uses citations from:
- FaceForensics++
- VGGNet and ViT papers
- Hugging Face Transformers
- Scikit-learn

Refer to the `References` section in the LaTeX file for details.

## ✍️ Author

**Pankaj Sheokand**  
Roll No: 102203410  
Email: pankajsheokand2005@gmail.com  
Thapar Institute of Engineering and Technology

## 📌 Future Work

- Incorporate audio-visual multimodal detection
- Test hybrid models on larger datasets
- Apply attention heatmaps (e.g., Grad-CAM) for explainability

## 🧾 License

This project is for academic and research purposes. You may use and adapt the code with proper citation.

```
