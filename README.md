# Topic-Modeling
Topic Modeling of New York Times Company News

*News copy* folder contains data of 31 companies collected by the author. Each file has three columns: date, headline/title, summary.

*nltk_data* folder contains stopwords and lemmatizr used to preprocess the text data. 

*topic_model.ipynb* is the code that takes *apple-incorporated.txt* as an example, runs [HDP](https://en.wikipedia.org/wiki/Hierarchical_Dirichlet_process), [LSI](https://en.wikipedia.org/wiki/Latent_semantic_analysis), [LDA](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation) and LDA_Mod (LDA with optimized number of topics) four models and uses [coherence value](https://radimrehurek.com/gensim/models/coherencemodel.html) to evaluate the results. An interactive visualization is built through [pyLDAVis](https://github.com/bmabey/pyLDAvis) for demonstrating the results of LDA.

## Sample Output


## Reference
Thanks to the [Topic Analysis example of Gensim](https://markroxor.github.io/gensim/static/notebooks/gensim_news_classification.html) and SusanLi's resourceful [Machine Learning] repository. 



