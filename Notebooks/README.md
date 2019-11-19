# Jupyter Notebooks Folder
---
These Jupyter Notebooks detail the code employed in the development of the data included in the database using Natural Language Processing. The base model employed was Spacy's medium Spanish model (es-core-news-ml), which was originally trained on news and Wikiner data. We trained it on a subset of our own texts to improve results and modified the pipeline to improve results on early modern Spanish.

## Recommended Order

These notebooks each work through a phase of the NER process. Though they can be read independently, a beginner might need to follow a certain order to understand the process. We recommend:

1. [Training Spacy's Model](Notebooks/Training Spacy's NER.ipynb) Guides you through the process of training the model, and performs a simple evaluation of the results.
1. [Adding a Custom Component to the Pipeline](Notebooks/Training Spacy's NER.ipynb) Explores the addition of a new pipeline component, here a normalized dictionary that modifies the "norm" attribute of each token, thus modifying the vector representation that the NER model is later trained with.
1. Evaluation notebooks. These notebooks explore different methods of evaluation of the training results, accounting for variations in the training and testing data by repeatedly training on different samples of the data.
    -[Evaluating Spacy NER (Out of the Box Model)](Notebooks/Evaluating Spacy NER (Out of the Box Model).ipynb)
    -[Evaluating Spacy NER Repeated Random Sub-Sampling (Trained Model with and without normalized dictionary)](Evaluating Spacy NER Repeated Random Sub-Sampling (Trained Model with and without normalized dictionary).ipynb)
    -[Evaluating Spacy NER K-fold Cross Validation (Trained Model with and without normalized dictionary)](Notebooks/Evaluating Spacy NER K-fold Cross Validation (Trained Model with and without normalized dictionary).ipynb)
