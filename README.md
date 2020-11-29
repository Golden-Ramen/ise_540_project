# ise_540_project: Covid-19 Vaccine Hesistancy analysis
## Yuesheng Luo, Linzhi Xi, Yifan He
This Repository includes the code and dataset used in Covid-19 Vaccin Hesitancy Analysis
### data_prepare.ipynb 
This file is for first step analysis of data distribution, getting to know the percentage of useful data and informations for the data cleaning step. 

### clean_text.ipynb

### Classifier_Yuesheng_Luo.ipynb
The file includes code for vectorizing tweets to sentence vectors and training with prediction models. 
Execute the TFIDF tokenization and Word2Vec embedding seperatly to get different vectorization for model training. 'Model Selection' block will give the metrics for each supervised learning method. 'Select Model Parameter' block returns the best parameter of the selected model. 'Prediction' generates the predicted result in .pkl format.\

### geo-location.ipynb
This file expores correlation between political preference and vaccine sentiments in each data.
It requires the user_loc feature in tweets, and stantardize location with geotext and other procedures. Two maps are drawn, showing the percentage of negative sentiments and percentage of republican poll in each states.

### Clustering_LSTM.ipynb
The file is for clustering part of the predictions of LSTM.
It includes generating total negative and positive tweets, doing feature extraction and K-means on two kinds of tweets and outputting sample tweets of each cluster.
The WordCloud of each cluster's sample tweets is plotted in 'Feature Extraction & KMeans Clustering' block.
