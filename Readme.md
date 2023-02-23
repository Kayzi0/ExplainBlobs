# Rule-based explanations of CNN classifiers using regional features

This is the repisitory corresponding to the paper 'rule-based explanations of CNN classifier using regional features'. Note that this is **not** production-grade code. It is prmarily structured into two different notebooks, namely `model_train.ipynb` and `regression.ipynb`. Comments have been provided to guide you through the process. It is strongly recommended to not just run the entire notebook at once, but to go through it step by step.

## How to use
1. Install the required libraries by running `pip install -r requirements.txt` in your environment
2. (Optional) install the right CUDA version and its dependencies for Tensorflow 2.10.

If you want to train your own model, run `model_train.ipynb` and then save the model. Otherwise, load one of the provided models in `regression.ipynb` and just use that notebook. Recommendations for all branches are given below.

### Branches
Branches provided are the following:
* main: contains the readme, the requirements and the blobs toy dataset
* blobs: contains the blobs toy dataset, up to date with main
* cells: contains the malaria cells dataset. Note that to use this branch, the dataset must first be downloaded from the kaggle repository: https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria
* distributions: contains a new dataset based on probability distributions

Please note that the branches are to be seen as fairly seperate, as the different dataset necessitate different feature extractions. Merging branches is thus **not advised**.

### Recommended model for each dataset:

* blobs: model40_padding
* cells: cells/model40
* distributions: model30_distro
