# Topic modelling with Spacy, Gensim and Textacy

The jupyter notebook '*topic-modelling.ipynb*' contains the following sections:

- Initialize: Setting up environment and loading data.
- Text extraction. Phrase and tokens extraction with Gensim and Spacy.
- Topic modelling. Using Textacy's LDA model.
- Data processing. Calculating data for visualization and export.
- Model evaluation. A collection of visualizations of the resulting topics.
- Export data. The data can be used for creating more visualization or import into a graph.


### General concept  
The emphasis in this notebook is on facilitating an iterative process where you can easily adjust stopwords and number of topics. Furthermore it contains features to re-focus on sub topics and thereby create a hierachy of topics.

### Input  
'data-in/tb_data.tsv' contains ~2100 scientific articles with the following properties: doi/title/abstract/keywords.

### Output 
Start by looking at the notebook: "topic-modelling.ipynb". Somewhere down the file you will find the 'visualization' section that gives an overview of the modelling data.  

Most of the other files in the output data directory (data-out/) is exported to be used as input in other projects. If you are interested in understanding the modelled topics more in detail you may look at 'tb_main_doc-top.html' output directory which contains a list the 15 most relevant articles for each topic.

### Caveat  
Topic modelling using LDA is an stochastic algorithm which will produce (slightly) different results even when run on the same data. The exact same results can therefore not be reproduced. 

### Inspiration
- https://github.com/skipgram/modern-nlp-in-python/blob/master/executable/Modern_NLP_in_Python.ipynb
- https://github.com/bhargavvader/personal/tree/master/notebooks/text_analysis_tutorial  
- Textacy Topic Modelling: https://github.com/chartbeat-labs/textacy == https://chartbeat-labs.github.io/textacy/index.html + http://textacy.readthedocs.io/en/latest/api_reference.html#module-textacy.tm.topic_model