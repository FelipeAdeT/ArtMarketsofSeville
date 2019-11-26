# Art Markets of Seville Database

---
            
**Background**

During the 16th and 17th centuries, Seville, Spain was the locus of the world's largest trade flows. From 1503 to 1717, it housed the Casa de Contratación, the institution that centralized trade between Europe and the Spanish colonies in the Americas. As a result, the city ballooned in wealth and population; with the specialization in trade, Sevillian artists started exporting their works abroad. 

**Uses**

This github repository is meant as a standalone project, but also as a resource for those conducting similar Humanities initiatives. If you are working on archival documentation in historical languages and ways of extracting their information computationally through NER, this provides a model and resources that can be tailored to your needs. It provides some directly usable resources for documents in early modern Spanish, created for a database comprised primarily of notarial and parish documents from the city of Seville.

**Data Source**

This database compiles information from 20 volumes of sources published throughout the 19th and 20th centuries in Seville. They compile data from several Sevillian archives on the activities of various local painters, sculptors, gilders, stonemasons, and architects, among other less common occupations. The books were OCR scanned, corrected for mistakes, and then divided into texts using OpenRefine. Texts are stored as individual records within the database and usually (though not always) refer to a single archival document, either in transcription or summarized form. These texts are often accompanied by footnotes and comments that are included as an attribute of the text in the database. Where possible, we have included the archival reference to the original source, to the extent provided by the researchers that edited the published volumes.

**Data Gathering**

The database is not only a repository of documents, but meant to dissect the information these documents contain. Different tables have been developed to register the actors, locations, objects, dates and money amounts present in any document, as well as the attributes of the document itself (archival reference, bibliographic source, footnotes and comments). Information on entities was extracted using the Named Entity Recognizer made available by Spacy (the medium Spanish model, es_core_news_ml). This model was trained on a set of training data tagged manually on DataTurks.com, improving the results, and the results were later revised.

**Basic Facts**
1. Thus far, the database incorporates 8,629 texts extracted from published archival documentation from Seville.
1. Data encompasses the 15th to the 19th centuries, with the highest volume of data focused on the 16th and 17th centuries.
1. These texts are transcriptions or summaries that usually refer to one archival document, but occasionally summarize several.
1. The texts have comments from the editors that provide additional information and occasionally refer to further archival documents than the one described in the main body.

**GitHub Repository**

This Github repository is meant to record the process of development of the database, including code used, training sets, output and further resources.

[Document Viewer](DocumentViewer.html)

**Proprietary Notice**

This project was developed by Felipe Álvarez de Toledo as part of a Ph.D. dissertation in the department of Art, Art History and Visual Studies at Duke University and as part of DALMI, the Duke, Art, Law and Markets Initiative. 

**License**

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/80x15.png" /></a><br />This project is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. This license applies to the database and its contents and the resources made available in this repository. It does not apply to the texts included in the database themselves, which were taken from published sources.
