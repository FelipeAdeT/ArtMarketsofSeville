# NER Resources

Named Entity Recognition is the process of extracting and labeling real-world entities with proper names in a set of texts. Examples of entities to be extracted can be people, locations, organizations, and even monetary amounts, dates, and a long etcetera of options.

Statistical models for NER are trained on corpora of texts. Those readily available online are usually trained on modern samples of news articles or on similarly standardized genres. We have found that these models can be used on historical texts, but results can greatly be improved.

In this project, we have used [Spacy's medium Spanish Model](http://www.spacy.io) to analyze historical Spanish texts, and we have experimented with several ways to improve its predictions. We have tried to improve accuracy and recall on existing tags (person, location, organization) and new tags (date, monetary amount, object) which whe have seen used in the more developed English models.

We have included a series of Jupyter notebooks documenting our process in this repository, accessible via the links below. They assume you have a basic knowledge of the Spacy library (if not, learn [here](https://spacy.io/usage/spacy-101)).

**Index**

1. [**Training Spacy's Model**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/TrainingSpacy's%20NER.ipynb) guides you through the process of training the model, and performs a simple evaluation of the results.
1. [**Adding a Custom Component to the Pipeline**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/Adding%20a%20Custom%20Pipeline%20Component%20on%20Spacy%20(normalized%20dictionary).ipynb) explores the addition of a new pipeline component, here a normalized dictionary that modifies the "norm" attribute of each token, thus modifying the vector representation that the NER model is later trained with.
1. **Evaluation notebooks** These notebooks explore different methods of evaluation of the training results, accounting for variations in the training and testing data by repeatedly training on different samples of the data.

    -[**Evaluating Spacy NER (Out of the Box Model)**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/Evaluating%20Spacy%20NER%20(Out%20of%20the%20Box%20Model).ipynb)
    
    -[**Evaluating Spacy NER Repeated Random Sub-Sampling**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/Evaluating%20Spacy%20NER%20Repeated%20Random%20Sub-Sampling%20(Trained%20Model%20with%20and%20without%20normalized%20dictionary).ipynb)
    
    -[**Evaluating Spacy NER K-fold Cross Validation**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/Evaluating%20Spacy%20NER%20K-fold%20Cross%20Validation%20(Trained%20Model%20with%20and%20without%20normalized%20dictionary).ipynb)
    
1. [**Exporting and saving the data**](https://github.com/FelipeAdeT/ArtMarketsofSeville/blob/master/Notebooks/Saving%20NER%20 output%20to%20file-Copy1.ipynb)
