# Topic-Modeling
Topic Modeling of New York Times Company News

*News copy* folder contains data of 31 companies collected by the author. Each file has three columns: date, headline/title, summary.

*nltk_data* folder contains stopwords and lemmatizer used to preprocess the text data. 

*topic_model.ipynb* is the code that takes *apple-incorporated.txt* as an example, runs [HDP](https://en.wikipedia.org/wiki/Hierarchical_Dirichlet_process), [LSI](https://en.wikipedia.org/wiki/Latent_semantic_analysis), [LDA](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation) and LDA_Mod (LDA with optimized number of topics) four models and uses [coherence value](https://radimrehurek.com/gensim/models/coherencemodel.html) to evaluate the results. An interactive visualization is built through [pyLDAVis](https://github.com/bmabey/pyLDAvis) for demonstrating the results of LDA.

## Sample Output
### 1. Coherence Value Comparison
<img src = "Images/Coherence%20Value%20-%20Models.png" height = "400">

#### Comments
Coherence value is calculated to evaluate the four models’ performance. It can be easily worked out using a built-in function in Gensim and the higher the coherence value, the more human interpretable the generated topics are. The experiment results of different company’s data were similar. Hence, only one result was shown below. 
The y-axis represents the coherence value of each model and the x-axis is the list of models. Typically, HDP model performs more than two time better than the other three models. LSI is slightly better than LDA or LDA_Mod. LDA and LDA_Mod receive a similar coherence value as we actually know in advance the optimal number of topics. 

### 2. Visualization of LDA result
<img src = "Images/Apple%20LDAViz.png" height = "400">

#### Comments
Apple Inc. is perhaps one of the most prominent technology companies. As we could tell from the graph on the left, three circles represent three most relevant topics and they have large coincided area, which suggest some evident focus of Apple’s news. The term-topic bar chart on the right captures Apple’s main products: “computer”, “iphone”, “mac”, “ipod”. Its core competency lies on “tech”, “patent”, “software” and “apps”; its direct competitors include “google” and “microsoft”.

## Reference
Thanks to the [Topic Analysis example of Gensim](https://markroxor.github.io/gensim/static/notebooks/gensim_news_classification.html) and SusanLi's resourceful machine learning repository - (https://github.com/susanli2016/Machine-Learning-with-Python).



