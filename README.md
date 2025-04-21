# MediScan AI

## Early Disease Detection Through Multi-modal Medical Imaging Analysis

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Overview

MediScan AI is an advanced medical diagnostic system that leverages artificial intelligence to analyze multiple imaging modalities (X-rays, MRIs, CT scans) alongside clinical reports for early disease detection. The system focuses on conditions prevalent in Nigeria, addressing the critical shortage of radiologists through AI-powered diagnostic assistance.

## Features

- **Multi-modal Analysis**: Integration of X-ray, MRI, and CT scan processing
- **Report Text Analysis**: Extraction of key clinical indicators from medical reports
- **Early Detection Pipeline**: Specialized models for stroke, tuberculosis, and cancer
- **Explainable Results**: Heatmap visualizations highlighting areas of concern
- **Offline Capability**: Functions in low-connectivity environments
- **Responsive Design**: Works across various devices including mobile phones

## Technology Stack

- **Backend**: Python, TensorFlow/PyTorch, FastAPI
- **Frontend**: JavaScript, React
- **Deployment**: Docker, Progressive Web App
- **Data Processing**: OpenCV, MONAI, PyDicom
- **NLP**: Transformers, BioClinicalBERT

## Installation

```bash
# Clone the repository
git clone https://github.com/tafolabi009/mediscan-ai.git
cd mediscan-ai

# Set up Python environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up frontend
cd frontend
npm install
npm run build
cd ..

# Run development server
python run.py
```

## Usage

1. Upload medical images (X-ray, MRI, CT scan)
2. Upload clinical reports (optional)
3. Select target conditions for analysis
4. Review AI-generated diagnostic suggestions
5. Export results as PDF report

## Model Architecture

MediScan AI employs a multi-stage architecture:

1. **Image Processing**: Specialized vision transformers for each imaging type
2. **NLP Module**: BioClinicalBERT for medical report analysis
3. **Feature Fusion**: Cross-attention mechanisms correlating findings across modalities
4. **Decision Engine**: Condition-specific classifiers with confidence scoring

## Dataset

The model is trained on the following datasets:
- CheXpert for chest X-rays
- MIMIC-CXR for radiological reports
- Nigerian-specific medical imaging datasets
- Synthetic data augmentations for rare conditions

## Project Impact

MediScan AI addresses critical healthcare challenges in Nigeria:
- Early detection of prevalent diseases
- Support for healthcare workers in areas with limited specialist access
- Standardization of diagnostic quality across different healthcare facilities
- Reduced diagnostic errors through multi-modal verification

## Team

- Afolabi - Team Lead/ AI Model Development
- Ifeoluwa - Frontend Development

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- RUNACOSS and DATICAN for organizing this competition
- Redeemer's University for support and resources
- Open source medical imaging community for datasets and baseline models
