# MediScan

**MediScan** is an AI-enabled medical diagnostics application that combines predictive models for heart disease and lung cancer with a modern web interface.

---

## 🚀 Project Overview

- **Backend**: Flask API serving prediction endpoints for heart disease and lung cancer.
- **Frontend**: React application for interactive user input and prediction result visualization.
- **Models**: Pre-trained machine learning models stored under `src/backend/models/`.
- **Training assets**: Jupyter notebooks for model development and validation are available in `training/`.

---

## 📁 Repository Structure

```text
MultiDiseasePrediction/
├── README.md
├── requirements.txt
├── RESTRUCTURING_CHECKLIST.md
├── src/
│   ├── backend/
│   │   ├── app.py
│   │   ├── config.py
│   │   ├── models/
│   │   │   ├── heart.pkl
│   │   │   └── lung_cancer_detection_model.keras
│   │   ├── routes/
│   │   │   ├── __init__.py
│   │   │   ├── heart.py
│   │   │   └── lung.py
│   │   └── uploads/  (runtime image uploads)
│   └── frontend/
│       ├── package.json
│       ├── public/index.html
│       └── src/
│           ├── App.js
│           ├── App.css
│           ├── index.js
│           └── index.css
└── training/
    ├── Heart_Disease_Prediction.ipynb
    ├── Lung-Cancer-Detection-using-CNN-V2.ipynb
    └── tests/
        ├── test_image.jpeg
        ├── test_lung.py
        ├── test_model.py
        └── test_real.py
```

---

## ✅ Key Features

- Heart disease prediction through structured clinical data.
- Lung cancer prediction using image-based classification.
- Clean separation of API, model assets, and UI.
- Notebook-driven experimentation for reproducibility.

---

## 🛠️ Prerequisites

- Python 3.10+ (recommended)
- Node.js 16+ and npm
- Git

---

## ⚙️ Installation

### 1. Set up Python environment

```bash
cd MultiDiseasePrediction
python -m venv venv
```

Activate the environment:

- PowerShell:
  ```powershell
  .\venv\Scripts\Activate.ps1
  ```
- Command Prompt:
  ```cmd
  .\venv\Scripts\activate.bat
  ```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 2. Install frontend dependencies

```bash
cd src/frontend
npm install
```

---

## ▶️ Run the Application

### Backend

```bash
cd src/backend
python app.py
```

The API should be available at:

- `http://localhost:5000`

### Frontend

```bash
cd src/frontend
npm start
```

The React UI should open at:

- `http://localhost:3000`

---

## 🧪 Testing

There are test assets in `training/tests/` for verifying model-related workflows.

Run Python-based tests using your preferred test runner, for example:

```bash
python -m pytest training/tests
```

> Note: If `pytest` is not installed, add it to `requirements.txt` or install it manually.

---

## 📌 Important Notes

- The repository includes pre-trained models in `src/backend/models/`.
- Training datasets are not included due to size and licensing restrictions.
- If you want to re-run training notebooks, place your datasets under `training/data/`.

---

## 📚 Optional Enhancements

- Add dataset download links in `training/`.
- Document backend API endpoints and request formats.
- Add frontend screenshots or demo instructions.

---

## 📝 Additional Resources

- `RESTRUCTURING_CHECKLIST.md` — guidelines for project refactoring and organization.

---

## 🙌 Contact

For questions or improvements, update this README or open an issue in the repository.
