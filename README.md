## Description
Official implementation of the paper: *Machine learning for Anxiety and Depression Profiling and Risk Assesment in the aftermath of an emergency*

## Getting started

1. Create conda environment *ds2024*
   
   `conda create --prefix ./ds2024`

2. Activate your local environment

    `conda activate .\ds2024`

3. Update conda environment from environment.yml file

    `conda env update --prefix ./ds2024 --file environment.yml`

4. (If required) Install additional python libraries

    `conda install <python_library>`

4. (For development) Exporting and sharing local environment

    `conda env export --from-history> environment.yml`--prune`

5. Add *./ds2024* to .gitignore

6. Initialize Git repository

    `git init`

## Code
Folder `src` contains the `utils.py` that contain the developed functions. functionsfile that generates trained models over folds. Results are stores in the folder `results`. In the `notebook` folder there is the `analysis.ipynb` file that generates all the figures.

```
├──  data  - COVICAT dataset and codebook
|
├──  reports/figures           - This folder contains all the generated figures
│ 
├──  notebooks
│   ├── train.ipynb            - Code for the training of ML models
|   └── evaluation.ipynb       - Code for the evaluation and explainability of ML models
│
├── results/                   - this folder contains final results to report performance and explainability
│   └── G_anxietyscore/XGBoost
│   └── G_depressionscore/XGBoost
|   |
|   └── Logistic Regression
|   └── Multi-Layer Perceptron
|   └── Naive Bayes
|   └── Random Forest
|   └── Support Vector Machines
|   └── XGBoost
|
├── models/                    - this folder stores trained ML models
│   └── G_anxietyscore/
│   └── G_depressionscore/
|   └── G_totalscore/
│
├── cv_data/                   - this folder stores post-processed folded data
│   └── G_anxietyscore/
│   └── G_depressionscore/
|   └── G_totalscore/
|
├── src                        - this folder contains utility functions.
│   └── utils.py
│   └── config.py
│
├── config.yaml                - Configuration file (Parameter definition)
```

## Data
Data is not publically available.
    







