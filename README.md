# Repository Contents

## 1. CoClusertingRandomisedSearch.ipynb
- **Focus**: Collaborative filtering using the Co-Clustering algorithm.
- **Features**:
  - Utilizes the `surprise` package for building and evaluating the recommendation system.
  - Data used: `netflix-5k.train.feather`, `netflix-5k.validation.feather`, and `netflix-5k.movie_titles.feather`.

## 2. KNNBasicRandomisedSearch.ipynb
- **Focus**: Collaborative filtering using the KNNBasic algorithm.
- **Features**:
  - Uses the `surprise` package for model training and evaluation.
  - Data used: `netflix-5k.train.feather`, `netflix-5k.validation.feather`, and `netflix-5k.movie_titles.feather`.

## 3. S3891013-A3-notebook.ipynb
- **Focus**: An instructional notebook based on the Netflix Prize dataset.
- **Features**:
  - Provides an overview of the dataset, including pre-defined train and validation splits.
  - Links to external readings related to the Netflix Prize.
  - Discusses data analysis techniques and points to official documentation.

## 4. SVDRandomisedSearch.ipynb
- **Focus**: Singular Value Decomposition (SVD) algorithm for collaborative filtering.
- **Features**:
  - Employs the `surprise` package for model building and evaluations.
  - Data used: `netflix-5k.train.feather`, `netflix-5k.validation.feather`, and `netflix-5k.movie_titles.feather`.

---

**Note**: All notebooks in this repository utilize datasets from the Netflix Prize and primarily focus on collaborative filtering techniques using different algorithms available in the `surprise` package.


## Results

### CoClusertingRandomisedSearch.ipynb
- Best score: 0.8828
- Best parameters:
  - `n_epochs`: 35
  - `n_cltr_u`: 7
  - `n_cltr_i`: 9

### KNNBasicRandomisedSearch.ipynb
- Best score: 0.9009
- Best parameters:
  - `sim_options`: 
    - `name`: pearson_baseline
    - `user_based`: False
    - `shrinkage`: 150
    - `min_support`: 2
  - `min_k`: 1
  - `k`: 40

### S3891013-A3-notebook.ipynb
- Dataset contains 1,287,017 rows with columns: `userID`, `movieID`, and `rating`.
- Rating statistics:
  - Mean: 3.610
  - Median: 4.0
  - Standard Deviation: 1.045
  - Range: 1.0 to 5.0

### SVDRandomisedSearch.ipynb
- Best score: 0.8447
- Best parameters:
  - `n_factors`: 225
  - `n_epochs`: 110
  - `biased`: False
  - `init_std_dev`: 0.2
  - `lr_all`: 0.005
  - `reg_all`: 0.055
  - `init_mean`: 0.25
