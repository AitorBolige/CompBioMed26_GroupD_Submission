# DataScience Seminars

Project submission for the Data Science Seminars course. The project explores
QRS signal data, performs feature extraction and Site-of-Origin (SOO)
standardization, and trains classification models to analyze and predict
outcomes from the processed signals.

## Repository structure

```
.
├── data/                      # Raw and processed datasets (.mat, .pkl)
├── models/                    # Trained model files (model.1 … model.5)
├── notebooks/
│   ├── project_code.ipynb     # Main analysis and modeling notebook
│   └── qrs_signals_function/  # Per-patient QRS signal arrays (.npy)
├── output/                    # Generated figures and result plots
└── soo_standarization/        # Standardized Site-of-Origin (SOO) tables (.csv)
```

## Contents

- **data/** — Source data, including the QRS database, simulation data, and the
  corrected full dataset used throughout the analysis.
- **notebooks/project_code.ipynb** — End-to-end workflow: data loading,
  preprocessing, feature extraction, model training, and evaluation.
- **models/** — Serialized trained models produced by the notebook.
- **output/** — Figures generated during analysis (confusion matrices, feature
  importance, PCA separability, error analysis, etc.).
- **soo_standarization/** — Standardized Site-of-Origin reference tables.

## Getting started

1. Open `notebooks/project_code.ipynb` in Jupyter.
2. Make sure the `data/` directory is present alongside the notebook.
3. Run the cells in order to reproduce the preprocessing, training, and figures.

## Requirements

The notebook uses the standard Python data-science stack, typically including:

- `numpy`, `pandas`, `scipy`
- `scikit-learn`
- `matplotlib`
- `jupyter`

Install them with:

```bash
pip install numpy pandas scipy scikit-learn matplotlib jupyter
```
