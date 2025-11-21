# AI-Medical-Diagnosis

Internship project for Edunet Foundation — a small collection of machine learning notebooks,trained models, and a simple application for exploring automated medical-diagnosis predictions.

This repository focuses on predicting/identifying several conditions using classic ML models:
- Diabetes
- Heart disease
- Parkinson's disease
- Lung cancer/disease
- Hypothyroid (Thyroid)

**Directory overview**
- `Medical diagnosis using AI/` : main project folder containing notebooks, `app.py`, datasets, and saved models.
	- `app.py` : small web app (Flask) that loads saved models and exposes prediction endpoints / simple UI.
	- `*.ipynb` : Jupyter notebooks with EDA, preprocessing, model training and evaluation for each condition.
	- `Datasets/` : raw and preprocessed CSV datasets used for experiments.
	- `Models/` : serialized model files (e.g. `.sav`) used by `app.py` and for inference.

**Quick start — run the app (Windows PowerShell)**
1. Create and activate a virtual environment:

```powershell
python -m venv .venv; 
.\.venv\Scripts\Activate.ps1
```

2. Install common dependencies (add more if your notebooks require them):

```powershell
pip install -U pip
pip install numpy pandas scikit-learn flask joblib matplotlib seaborn jupyter
```

3. Run the app:

```powershell
python "Medical diagnosis using AI\app.py"
```

Open the address printed by the app (typically `http://127.0.0.1:5000`) in your browser.

Note: `app.py` expects the trained model files to be present in `Medical diagnosis using AI/Models/`.

**Working with the notebooks**
- Open the notebooks found in `Medical diagnosis using AI/` with Jupyter Lab/Notebook.
- Each notebook includes data loading (from `Datasets/`), preprocessing steps, model training,
	evaluation, and instructions for saving the final model to `Models/` using `joblib` or `pickle`.

**Datasets and Models**
- Datasets are stored under `Medical diagnosis using AI/Datasets/`. Examples:
	- `diabetes_data.csv`
	- `heart_disease_data.csv`
	- `parkinson_data.csv`
	- `survey lung cancer.csv` and preprocessed variants
- Trained models are under `Medical diagnosis using AI/Models/`, e.g. `diabetes_model.sav`.


---


