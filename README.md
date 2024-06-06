# PlantTraits2024 – MLiP Project – by Noodle Nappers

Welcome to the Noodle Nappers project repository, dedicated to the 2024 Machine Learning in Practice (MLiP) course at Radboud University. This repository focuses solely on the [Kaggle competition](https://www.kaggle.com/competitions/planttraits2024) aimed at predicting plant traits using photographs and ancillary geodata. Our work here aims to contribute to the understanding of the global patterns of biodiversity.

**Authors: Luppo Sloup, Dick Blankvoort, Tygo Francissen (MLiP Group 9)**

## Overview

The goal of this competition is to develop a deep learning-based regression model, supplemented with ancillary geodata, to predict plant traits from plant photographs. By accurately predicting these traits, this project can aid researchers in understanding how plant traits and as such entire ecosystems will react to climate change.

## Our Work

Our work includes multiple notebooks and data sets, which are explained in more detail below.

### Notebooks

For the sake of convenience, we opted to only use Kaggle notebooks in this competition without a dedicated GitHub workflow. We did however communicate all changes excellently to each other, which worked great for us. In our project, many notebooks were created. We list the most important ones from our accounts on Kaggle below.

We utilized these notebooks to modify the EfficientNet B0 starter for training and inference:

- [Train Notebook](https://www.kaggle.com/code/tygofrancissen/train-notebook)
- [Inference Notebook](https://www.kaggle.com/code/tygofrancissen/inference-notebook)

Furthermore, we modified the HMS ensemble of EfficientNet and ResNet to fit our ensemble model with these notebooks:

- [HMS Multiple Model Ensemble Original](https://www.kaggle.com/code/luepoe/hms-multiple-model-ensemble-4-notebooks-19b844)
- [IIACT Training HMS Workflow](https://www.kaggle.com/code/luepoe/iiact-training-hms-workflow)
- [Master Training HMS Workflow](https://www.kaggle.com/code/luepoe/master-training-hms-workflow)

As we added more models to the ensemble, we needed to modify and search through more notebooks:

- [IIACT Ensamble Features Head Starter](https://www.kaggle.com/code/luepoe/iiact-ensamble-features-head-starter)
- [Wavenet Starter](https://www.kaggle.com/code/luepoe/wavenet-starter-lb-0-66)
- [WaveNet Training](https://www.kaggle.com/code/luepoe/lb-0-46-dilatedinception-wavenet-training)
- [WaveNet Inference](https://www.kaggle.com/code/luepoe/lb-0-46-dilatedinception-wavenet-inference)
- [Catboost Starter](https://www.kaggle.com/code/luepoe/catboost-starter-lb-0-67)

Finally, this notebook we created combines all models to create an ensemble and the submission:

- [IIACT Ensemble 7 Models](https://www.kaggle.com/code/luepoe/iiact-ensamble-7-models)

Note that this notebook has not been made public in order to keep our best-working code private, but it is available in this repository as `ensemble-7-models.ipynb`.

### Datasets

To be able to store augmented data, packages, and models, we created several data sets on Kaggle:

- [Brain Solver](https://www.kaggle.com/datasets/luepoe/brain-solver): This data set contains the whole Python package with all the code being pushed into this using GitHub workflows. There are almost 125 versions available of this package.
- [D2L Package](https://www.kaggle.com/datasets/tygofrancissen/d2l-package): This data set contains the necessary files to properly import the d2l package, as it is not available in Kaggle using offline mode.
- [Trained Model EfficientNet](https://www.kaggle.com/datasets/tygofrancissen/trained-model-effnet-mlip9): This data set contains all versions of trained models for our modified EfficientNet notebook.
- [Wav2vec/Filter EEGs and Spectograms](https://www.kaggle.com/datasets/dickblankvoort/w2v-specs): This data set contains the raw EEG data and spectograms after being processed with wav2vec, filters, or a combination.
- [Models Wav2Vec/Filter Training](https://www.kaggle.com/datasets/dickblankvoort/models-first-wav2vec-training): This data set contains a wide range of models that were stored after being trained with the `Wav2vec/Filter EEGs and Spectograms` data set mentioned above.
- [Catboost Model](https://www.kaggle.com/datasets/luepoe/catboost-model): This data set stores the trained models for CatBoost.
- [Dilated WaveNet](https://www.kaggle.com/datasets/luepoe/dilated-wavenet): This data set stores the trained models for WaveNet.
