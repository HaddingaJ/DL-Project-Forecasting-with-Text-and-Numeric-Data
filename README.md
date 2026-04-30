# DL-Project-Forecasting-with-Text-and-Numeric-Data
Code used for course project in the course INF 395T: Deep Learning and Multimodal Systems, Spring 2026

Authors: Manuel Diaz de la Fuente & Joost Haddinga

This repository contains the following files

- Text_Preprocessing.ipynb: Load and format transcripts. Provides formatted transcripts for multimodal processing
-
- Analysis_multimodal.ipynb: Build and evaluate multimodal dataset, architecture and model. Provides the final models, evaluation statistics and figures

- ric_sector_lookup.csv and SPX_leavers_joiners.xlsx are data files used for adding firm metadata


Running the notebooks should be carried out sequentially:

Analysis_multimodal relies on the transformed transcripts from Text_Preprocessing

Analysis_multimodal uses hyperparameters from the numeric architecture (not integrated but one may update the hyperparameters in case running the numeric architecture in a different way).

Python 3.10+ required to execute the notebooks.
