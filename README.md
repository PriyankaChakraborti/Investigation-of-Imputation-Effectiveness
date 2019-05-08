# Investigation-of-Data-Imputation-techniques-for-Extremely-Sparse-Features

We investigate multiple techniques for dealing with the common problem of massive missing data. To this end we explore two data sets from entirely disparate domains and numbers of entries, exploring the approach of imputing missing data one feature at a time. Our investigation shows that irrespective of the size of the dataset, it is very difficult to properly impute the missing data. However, some well known ML algorithms can produce worthy placeholder values for target prediction. In such cases their performance (evaluated by the mean squared error on the true target variable) is surprisingly sometimes comparable to, or even surpassed, by simple mean imputation or by bare bone removal of the row corresponding to the missing entries. As elaborated in the article, this is true even for cases where our true target is strongly correlated with the imputed feature. Finally, an experiment using MICE (Multiple Imputation by Chained Equations) on multiple columns of missing data in a medium size dataset results in results which far surpass the approach of removing rows missing any data.

The Zillow dataset used for the Single Column Imputation investigation can be downloaded from Kaggle on this page:<br>
https://www.kaggle.com/c/zillow-prize-1/data

The Facebook dataset used for the Single Column Imputation investigation and the Multi-Column Imputation investigation can be downloaded on this page:<br>
https://archive.ics.uci.edu/ml/datasets/Facebook+metrics
