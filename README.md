# DL-Project-Forecasting-with-Text-and-Numeric-Data
Code used for course project in the course INF 395T: Deep Learning and Multimodal Systems, Spring 2026

Authors: Manuel Diaz de la Fuente & Joost Haddinga

This repository contains the following files

- Text_Preprocessing.ipynb: Load and format transcripts. Provides formatted transcripts for multimodal processing
- Numeric_models.ipynb: Builds numeric models, performs hyperparameter tuning for each forecast horizon and evaluates results.
- Analysis_multimodal.ipynb: Build and evaluate multimodal dataset, architecture and model. Provides the final models, evaluation statistics and figures

- ric_sector_lookup.csv and SPX_leavers_joiners.xlsx are data files used for adding firm metadata


Running the notebooks should be carried out sequentially:

Analysis_multimodal relies on the transformed transcripts from Text_Preprocessing

Analysis_multimodal uses hyperparameters from the numeric architecture (not integrated but one may update the hyperparameters in case running the numeric architecture in a different way).

Python 3.10+ required to execute the notebooks.

## Time Series Sources:
- Consumer Price Index: https://fred.stlouisfed.org/series/CPIAUCSL
- Federal Funds Rate: https://fred.stlouisfed.org/series/DFF
- Industrial Production Index: https://fred.stlouisfed.org/series/INDPRO
- Unemployment Rate: https://fred.stlouisfed.org/series/UNRATE
- Economic Policy Uncertainty Index: https://fred.stlouisfed.org/series/USEPUINDXD
- VIX: https://fred.stlouisfed.org/series/VIXCLS

### Additional:

- VAR_exploratory: The statsmodel package was giving some concerning warnings when estimating the VAR, so we decided to check manually whether the parameters were being correctly estimated.