# Multi-omic generation

Collaborative project with l'INSEE aimed at generating omic data while considering other modalities, facilitating comprehensive data analysis and interpretation.

## Installation

To install the required dependencies, run the following command:

 ```bash
pip install -r requirements.txt
```

## Datasets

We study three modalities : expression, methylation, protein.
The function generate_datasets from the datasets.py file returns thee datasets for training, testing or both.

example:
```python
datasets = generate_datasets(suffix='5_diff', type='unpaired', train=True, test=False)
# Generate the dataloaders
dataloaders = [DataLoader(ds, batch_size=32, drop_last=True, shuffle=False) for ds in test_datasets]
```

## Models 

This repository provides implementations of several multi-omic generation models. Below, you'll find descriptions of two of them:

## Model 1

## Model 2



For training just run the training notebook  `train_models_1_and_2.ipynb`.

The trained model is store in the `./checkpoint` folder.

## Training report
