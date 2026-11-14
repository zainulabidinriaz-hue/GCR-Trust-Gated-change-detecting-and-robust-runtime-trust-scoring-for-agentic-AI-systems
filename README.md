# GCR-Trust: Supplementary Material

Code and data for the article *"GCR-Trust: Gated, change-detecting and robust runtime trust scoring for agentic AI systems"* by Zain Ul Abidin Riaz, Ayesha Riaz and Bilal Riaz.

## Files

| File | What it contains |
| --- | --- |
| `trust_sim.py` | Simulation script that produces every number in Tables 4 to 8 of the article: the baseline trust model (Experiments 1–3) and the comparison with GCR-Trust (Experiments 4–6). |
| `make_figures.py` | Draws all twelve figures of the article (Figures 1–12). Run it after `trust_sim.py`. |
| `results.json` | The exact output of `trust_sim.py`, so results can be checked without running the code. |
| `audit_coding_sheet.csv` | The validation audit (Table 2): each of the 50 framework–criterion scores (Y / P / N) with the supporting quotation or note from the audited paper. |

## Reproducing the results

Requirements: Python 3.9 or later, NumPy and Matplotlib.

```bash
pip install numpy matplotlib
python trust_sim.py
python make_figures.py
```

The script uses fixed random seeds (20261010 for Experiments 1–3 and 20261011 for Experiments 4–6), so it writes a `results.json` identical to the one in this repository. It runs in under a minute on an ordinary laptop.

## Citation

If you use this material, please cite the article (citation details will be added on publication).
