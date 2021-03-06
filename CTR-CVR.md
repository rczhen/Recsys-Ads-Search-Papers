# CTR & CVR Prediction

Click-trough Rate (CTR) and Conversion Rate (CVR) prediction, or saying user response prediction, have been a principal problem in recommender system, online advertising and web search. The two main threads are: 

1. From traditional ML models (Logistic Regression, Tree, Factorization Machine etc.) to deep learning models
2. Better utilize features: 
    * Explore useful features
    * Perform features interactions: Towards altomatic feature interaction extraction and higher-order feature interaction. Although feature engineering and lower-order feature interactions are necessary sometimes. 
    * Weighted features or their embeddings

## 1. Feature interactions
### 1.1 Lower Order Feature Interaction

#### Factorization Machine (FM)
* FM 2010: [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf). 
Factorization Machine (FM) is proposed in 2010, prior to the boom of Deep Learning. At that moment, features are mostly represented by the sparse, high dimensional one-hot encoding, instead of the dense, lower dimensional feature embedding. Therefore, sparsity leads to difficulties when learning weights of feature interactions. FM solves this problem by "modeling all interactions between variables using factorized parameters. Thus they are able to estimate interactions even in problems with huge sparsity (like recommender systems) where SVMs fail". Nowadays FM also serves as feature latent vectors extractors (e.g. in DeepFM), as well as a tool to reduce the number of feature interactions coefficients (e.g. in Product-based Neural Network). 
* FFM 2016: [Field-aware Factorization Machines for CTR Prediction](https://www.csie.ntu.edu.tw/~cjlin/papers/ffm.pdf). 
* DeepFM 2017: [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/pdf/1703.04247.pdf). 
* xDeepFM 2018: [xDeepFM: Combining Explicit and Implicit Feature Interactions
for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf). 

#### Tree Models
* Facebook GBDT + LR 2014: [Practical Lessons from Predicting Clicks on Ads at
Facebook](https://quinonero.net/Publications/predicting-clicks-facebook.pdf). 
* Google Wide and Deep 2016: [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf). 

#### Product-based
* [Product-based Neural Network 2016](https://arxiv.org/pdf/1611.00144.pdf): 
* [Deep & Cross Network 2017](https://arxiv.org/pdf/1708.05123.pdf): 

### 1.2 Higher Order Feature Interaction

#### Transformer
* AutoInt 2018: [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/pdf/1810.11921.pdf)

## 2. Feature (Embedding) Weighted
* [Alibaba Deep Interest Network 2017](https://arxiv.org/pdf/1706.06978.pdf):
* [Sina FiBiNET 2019](https://arxiv.org/pdf/1905.09433.pdf):

## 3. Multi-Task
* [Alibaba ESSM 2018](https://arxiv.org/pdf/1804.07931.pdf): 
* [Alibaba ESSM2 2019](https://arxiv.org/pdf/1910.07099.pdf): 

## 4. Traditional ML Models Methods
* [Alibaba Multi Logistic Regression 2017](https://arxiv.org/pdf/1704.05194.pdf):

## 5. Exploitation and Exploration
* [Exploitation and Exploration in a Performance based Contextual Advertising System](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.297.8373&rep=rep1&type=pdf)