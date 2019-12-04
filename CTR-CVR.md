# CTR & CVR Prediction

Click-trough Rate (CTR) and Conversion Rate (CVR) prediction, or saying user response prediction, have been a principal problem in recommender system, online advertising and web search. The two main threads are: 

1. From traditional ML models (Logistic Regression, Tree, Factorization Machine etc.) to deep learning models
2. Better utilize features: 
    * Explore useful features
    * Perform features interactions: Towards altomatic feature interaction extraction and higher-order feature interaction. Although feature engineering and lower-order feature interactions are necessary sometimes. 
    * Weighted features or their embeddings

## Feature interactions
#### Factorization Machine (FM)
* [FM 2010](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf): 
* [FFM 2016](https://www.csie.ntu.edu.tw/~cjlin/papers/ffm.pdf): 
* [DeepFM 2017](https://arxiv.org/pdf/1703.04247.pdf): 

#### Tree Models
* [Facebook GBDT + LR 2014](https://quinonero.net/Publications/predicting-clicks-facebook.pdf): 
* [Google Wide and Deep 2016](https://arxiv.org/pdf/1606.07792.pdf): 

#### Product-based
* [Product-based Neural Network 2016](https://arxiv.org/pdf/1611.00144.pdf): 

## Feature (Embedding) Weighted
* [Alibaba Deep Interest Network 2017](https://arxiv.org/pdf/1706.06978.pdf):
* [Sina FiBiNET 2019](https://arxiv.org/pdf/1905.09433.pdf):

## Multi Task
* [Alibaba ESSM 2018](https://arxiv.org/pdf/1804.07931.pdf): 
* [Alibaba ESSM2 2019](https://arxiv.org/pdf/1910.07099.pdf): 

## Traditional ML Models Methods
* [Alibaba Multi Logistic Regression 2017](https://arxiv.org/pdf/1704.05194.pdf):
