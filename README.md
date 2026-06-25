# AI Programming Foundations Project

Author: Sukh Sandhu

## Project Description

This project builds a reusable Python data workflow for the scikit-learn Wine recognition dataset. The workflow includes dataset ingestion, two cleaning functions, an exploratory analysis function, three visualizations, and a final interpretation section.

## How to Run

1. Install dependencies:
   `pip install -r requirements.txt`
2. Start Jupyter Notebook:
   `jupyter notebook`
3. Open and run:
   `data_workflow.ipynb`

## Files

- `data_workflow.ipynb`: executable notebook with workflow sections.
- `data/wine_dataset.csv`: dataset used by the notebook.
- `figures/`: saved visualization outputs.
- `module_summary.pdf`: written summary with citations.
- `requirements.txt`: reproducibility file.

## Reflection: Bias From Poor Data Cleaning

Poor cleaning can introduce bias if rows are removed unevenly across wine cultivars, if missing values are filled in a way that changes class-level chemistry patterns, or if feature names are altered in ways that hide units or measurement meaning. In this workflow, cleaning was intentionally conservative: column names were standardized, duplicates were checked, and nonnegative measurement validation was applied without dropping valid observations.

## Future Integration Reflections

For a machine learning workflow, this project would need train-test splitting, preprocessing pipelines, metric selection, and validation checks. For neural-network preparation, the numeric predictors would need scaling and careful tensor conversion, while correlated variables would need monitoring for instability. An agentic automation layer could rerun ingestion, cleaning, and figure generation after a dataset update, then flag unexpected missingness or distribution drift for human review.
