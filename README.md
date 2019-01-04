# Topic-Modeling
Topic Modeling of New York Times Company News

The News folder contains data of 31 companies collected by the author. Each file has three columns: Date, Headline/Title, Summary.
The nltk_data folder contains stopwords and lemmatizr used to preprocess the text data. 
The topic_model.ipynb is the code that takes apple-incorporated.txt as an example, runs HDP, LSI, LDA and LDA_Mod (LDA with optimized number of topics) four models and uses Coherence Value to evaluate the results. An interactive visualization is built through pyLDAVis for demonstrating the results of LDA.

## Sample Output


## Reference
Thanks to the [Topic Analysis example of Gensim](https://markroxor.github.io/gensim/static/notebooks/gensim_news_classification.html) and [Machine Learning]  (https://github.com/susanli2016/Machine-Learning-with-Python) github repository.


