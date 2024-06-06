# PlantTraits2024 – MLiP Project – by Noodle Nappers

Welcome to the Noodle Nappers project repository, dedicated to the 2024 Machine Learning in Practice (MLiP) course at Radboud University. This repository focuses solely on the [Kaggle competition](https://www.kaggle.com/competitions/planttraits2024) aimed at predicting plant traits using photographs and ancillary geodata. Our work here aims to contribute to the understanding of the global patterns of biodiversity.

**Authors: Luppo Sloup, Dick Blankvoort, Tygo Francissen (MLiP Group 9)**

## Overview

The goal of this competition is to develop a deep learning-based regression model, supplemented with ancillary geodata, to predict plant traits from plant photographs. By accurately predicting these traits, this project can aid researchers in understanding how plant traits and as such entire ecosystems will react to climate change.

## Our Work

Our work includes multiple notebooks and data sets, which are explained in more detail below.

### Notebooks

For the sake of convenience, we opted to only use Kaggle notebooks in this competition without a dedicated GitHub workflow. We did however communicate all changes excellently to each other, which worked great for us. In our project, many notebooks were created. We list the most important ones from our accounts on Kaggle below (which are all publicly available).

We utilized this notebook to modify the Keras starter notebook, try out different versions of a stacked ensemble (V1-13), and to test different ImageNet models (V14-51):

- [Exploration Notebook](https://www.kaggle.com/code/dickblankvoort/planttraits2024-exploration-models)

Moreover, to compare different tabular data models and augmentations, we used the following notebook:

- [Tabular Model Notebook](https://www.kaggle.com/code/luepoe/tabular-data-training) **NOT PUBLIC YET CHANGE**

For implementing image segmentation, filtering by segmentation, and label-free segmentation, the following notebooks were used to run many tests:

- [Segmentation Notebook](https://www.kaggle.com/code/dickblankvoort/segmentation-notebook)
- [Label-free Segmentation/Filtering Notebook](https://www.kaggle.com/code/dickblankvoort/label-free-segmentation-filtering-attempts)

As we wanted to try more and large ranges of image augmentations, we used the following notebooks:

- [Plant Notebook](https://www.kaggle.com/code/tygofrancissen/plant-notebook)
- [Plant Notebook (small tests)](https://www.kaggle.com/code/dickblankvoort/plant-notebook)

Before creating an ensemble, we tried many changes in the ImageNet notebook to search for optimizations. This involved changing the loss, R2, LR calculations, adding segmentation. Also, things like a magnitude difference test were done:

- [INet Improve Notebook](https://www.kaggle.com/code/dickblankvoort/inet-improve-model)
- [INet Magnitude Notebook](https://www.kaggle.com/code/dickblankvoort/inet-magnitude-difference-test)

Our stacked ensemble was built by performing several tests in multiple notebooks, listed below:

- [Stacked Ensemble Notebook](https://www.kaggle.com/code/luepoe/stacked-ensemble) **NOT PUBLIC YET CHANGE**
- [Stacked Ensemble V2 Notebook](https://www.kaggle.com/code/luepoe/v2-stacked-ensemble) **NOT PUBLIC YET CHANGE**

For our ensemble, we wanted to use the EDA notebook on Kaggle, which we made many variations on:

- [EDA Filter Bad Pictures Notebook](https://www.kaggle.com/code/dickblankvoort/eda-filtering-out-bad-pictures)
- [EDA Alternative Swin Notebook](https://www.kaggle.com/code/dickblankvoort/eda-training-alternative-swin)
- [EDA Training Twice Notebook](https://www.kaggle.com/code/dickblankvoort/modified-planttraits2024-eda-training-re-training)
- [EDA Training Twice V2 Notebook](https://www.kaggle.com/code/tygofrancissen/modified-planttraits2024-eda-training-re-training)
- [EDA With TTA Notebook](https://www.kaggle.com/code/tygofrancissen/modified-planttraits2024-eda-training)

Finally, this notebook we created combines all models to create an ensemble and the submission:

- [Ensemble 7 Models](https://www.kaggle.com/code/dickblankvoort/ensemble-model)

### Datasets

To be able to store data and models to be used in mostly the ensemble, we created several data sets on Kaggle:

- [Botany Model](https://www.kaggle.com/datasets/tygofrancissen/botany-output): This data set contains the output for one of the use models in the ensemble.
- [CatBoost Model](https://www.kaggle.com/datasets/luepoe/tdt-catboost-best-0-15450): Contains the output weights for our best CatBoost model.
- [Pickled Plant Data](https://www.kaggle.com/datasets/dickblankvoort/plant-data-pickled): Used by EDA notebook to read data faster.
- [Bad Plant Pictures](https://www.kaggle.com/datasets/dickblankvoort/bad-plant-pictures): Contains a list of bad plant pictures according to CLIP model.
- [Stacked Ensemble Model](https://www.kaggle.com/models/dickblankvoort/stacked-ensemble-joblib): This data set contains the trained model for the LightGBM part of the LGBM+EDA stacked ensemble.
- [INet Optimized Model](https://www.kaggle.com/models/dickblankvoort/inet-model-optimized): Contains our optimized trained ImageNet model.
- [Trained Models](https://www.kaggle.com/models/dickblankvoort/top-10-models): This data set contains the trained model files for the highest performing EDA and multi-target regression.
- [EDA Pretrained Model](https://www.kaggle.com/models/dickblankvoort/eda-pretrained): Contains the EDA model pretrained to 6 epochs.
