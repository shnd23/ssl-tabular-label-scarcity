# When Does Self-Supervised Pretraining Help Tabular Models?

Code and results for the paper *When Does Self-Supervised Pretraining Help Tabular Models? A Study of Label Scarcity and Missing Data* — Sahand Mazrouei, Kharazmi University.

## Contents

```
notebook/Main_Notebook_final.ipynb   — full pipeline 
results/                             — pre-computed tables and statistics
```

The `results/` folder contains all tables from the paper as CSVs and a `summary_statistics.json` with the exact numbers used in the text, so you can verify without rerunning anything.

## Running the notebook

Open `Main_Notebook_final.ipynb` in Google Colab with a GPU runtime and run cells in order. Data is downloaded from OpenML automatically. Results are cached after each task, so re-running is fast.

Dependencies (installed in the first cell): PyTorch, scikit-learn, openml, xgboost, lightgbm, scipy, statsmodels, matplotlib, pandas, numpy.

## Datasets

14 OpenML classification tasks, using the official predefined train/test split (fold 0) for each.

| Task ID | Dataset | Classes | Missingness |
|---------|---------|---------|------------|
| 2079 | Eucalyptus | 5 | 4.3% |
| 3021 | Sick | 2 | 22.2% |
| 14954 | Cylinder Bands | 2 | 5.3% |
| 146800 | MiceProtein | 8 | 1.7% |
| 2 | Anneal | 5 | 0.0% |
| 15 | Breast-W | 2 | 0.2% |
| 29 | Credit-Approval | 2 | 0.6% |
| 3904 | JM1 | 2 | 0.0% |
| 7592 | Adult | 2 | 0.0% |
| 6 | Letter | 26 | 0.0% |
| 32 | Pendigits | 10 | 0.0% |
| 37 | Diabetes | 2 | 0.0% |
| 43 | Spambase | 2 | 0.0% |
| 53 | Vehicle | 4 | 0.0% |

## Citation

```
@article{mazrouei2026tabularssl,
  title={When Does Self-Supervised Pretraining Help Tabular Models? A Study of Label Scarcity and Missing Data},
  author={Mazrouei, Sahand},
  year={2026}
}
```

## License

MIT — see `LICENSE`.
