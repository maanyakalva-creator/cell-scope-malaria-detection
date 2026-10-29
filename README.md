# CELL SCOPE — AI Hematology & Malaria Diagnostics Suite

Cell Scope is an AI-powered diagnostic and screening web application designed for malaria detection in blood smear microscopy images.

---

## 🔬 Features

- **Single-Cell Classification**: High-accuracy malaria screening (Parasitized vs. Uninfected) using MobileNetV2 deep learning model.
- **Grad-CAM Explainability**: Visual heatmaps explaining the model's focus and confidence.
- **Full Smear Analysis**: Automated RBC segmentation, count, and multi-cell batch classification.
- **Stain Normalization**: Standardized microscopy color normalization (Reinhard algorithm).
- **Quality Check**: Automated blurriness, contrast, and illumination diagnostics.
- **Patient & Visit Records**: Database persistence for patient history and visit triage.
- **PDF Diagnostic Reports**: Automated, exportable clinical laboratory report generation.

---

## 🚀 Quick Start

### 1. Requirements

Ensure Python 3.9+ is installed.

Install the dependencies:

```bash
pip install -r requirements.txt
```

### 2. Run the Application

Start the Flask development server:

```bash
python app.py
```

Open your browser and navigate to:

```
http://localhost:5000
```

---

## 📁 Project Structure

```
├── app.py                  # Main Flask application backend
├── db.py                   # SQLite database manager for patient triage & records
├── gradcam.py              # Grad-CAM heatmap visualization
├── malaria_model.keras     # Trained MobileNetV2 model weights
├── quality_check.py        # Image quality verification (blur, brightness, contrast)
├── rbc_detection.py        # Blood smear cell segmentation & extraction
├── report.py               # PDF diagnostic report generator
├── stain_norm.py           # Reinhard stain normalization algorithm
├── train_model.py          # Model training pipeline
├── requirements.txt        # Python package dependencies
├── static/                 # Static assets (CSS, JavaScript)
└── templates/              # HTML frontend templates
```
