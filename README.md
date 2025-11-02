# Tabular Deep Learning vs Classical ML for Urban Land Cover Classification

[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue)](#setup)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](#license)
![Task: Land-Cover](https://img.shields.io/badge/Task-Land%20Cover%20Classification-7957d5)
![Modality: Tabular](https://img.shields.io/badge/Modality-Tabular-4c9)
![Methods: TabDL+ClassicalML](https://img.shields.io/badge/Methods-TabDL%20%2B%20Classical%20ML-ff7f50)
![Notebook](https://img.shields.io/badge/Interface-Jupyter%20Notebook-ffcc00)
[![Dataset](https://img.shields.io/badge/Dataset-Urban%20Land%20Cover-1f77b4)](#data)
[![Conference: NeurIPS 2025 MusIML](https://img.shields.io/badge/Conference-NeurIPS%202025%20MusIML-0b7285)](#reference)
[![Cite Us](https://img.shields.io/badge/Cite-See%20BibTeX%20below-6c757d)](#reference)
![Status: Reproducible](https://img.shields.io/badge/Status-Reproducible-success)

A concise, reproducible notebook comparing **tabular deep learning** with **classical ML** on an **urban land cover** dataset.

---

## Data
- **Dataset:** [UCI Urban Land Cover](https://archive.ics.uci.edu/dataset/295/urban+land+cover)
- Place raw files in `data/raw/`; the notebook writes processed files to `data/processed/`.
- Please respect the dataset’s license and terms of use.

---

## Setup
```bash
conda create -n ulc python=3.10 -y
conda activate ulc
pip install -r requirements.txt
```

> Minimal `requirements.txt`: numpy, pandas, scikit-learn, matplotlib, scipy, jupyter  
> (Optionally add xgboost, lightgbm, catboost, torch if used.)

---

## Quickstart
Run the notebook end-to-end to reproduce results and generate figures.

```bash
# Ensure required folders exist
mkdir -p data/raw data/processed outputs/figures notebooks

# Launch Jupyter and open the notebook
jupyter lab notebooks/Urban Land Cover Classification.ipynb
# or
jupyter notebook notebooks/Urban Land Cover Classification.ipynb
```

Expected outputs:
- `outputs/metrics.csv` — aggregated metrics (e.g., Accuracy, Macro-F1)  
- `outputs/figures/` — plots and confusion matrices

---

## Reference
M. Tabasum, T. Tasnim, M.E. Islam, A.Z.S.B. Habib,  
**“Tabular Deep Learning vs Classical Machine Learning for Urban Land Cover Classification,”**  
*NeurIPS 2025 The 5th Muslims in ML (MusIML) Workshop*. (Accepted)

**BibTeX**
```bibtex
@inproceedings{tabasum2025tabdlulc,
  title     = {Tabular Deep Learning vs Classical Machine Learning for Urban Land Cover Classification},
  author    = {Tabasum, Muntasir and Tasnim, Tanpia and Islam, Md. Ekramul and Habib, Al Zadid Sultan Bin},
  booktitle = {NeurIPS 2025 The 5th Muslims in ML (MusIML) Workshop},
  year      = {2025},
  note      = {Workshop paper}
}
```

---

## License
MIT License — free to use, modify, and distribute with attribution.  
Include a separate `LICENSE` file if you plan to share the repository publicly.

---

## Contact
**Muntasir Tabasum** · West Virginia University  
Department of Geology & Geography  
For issues or questions, please use GitHub Issues.

---

## Copyright
© 2025 Muntasir Tabasum. All rights reserved.  
If you use this repository or cite the results, please include the above reference.
