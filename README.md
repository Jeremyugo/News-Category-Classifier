## News-Category-Classifier

This repository contains a deep learning project where a custom keras function model was built to classify news categories using three (3) input features. 
The model was trained on 125,000 + instances with forty-two (42) categories as the target, and achieved a test set accuracy of `70%`, which is significantly 
higher that other [models](https://www.kaggle.com/datasets/rmisra/news-category-dataset/code?datasetId=32526&sortBy=voteCount) trained using using the same data, with the exception of notebooks:

- using a pre-trained BERT model with 335 million paramteters - 74% accuracy
- using eleven (11) classes as opposed to all forty-two (42) classes - 72% accuracy

![image](https://github.com/Jeremyugo/News-Category-Classifier/assets/36512525/cfe0172a-e8c2-46ee-b6bf-eb328aea4e55)

On the surface level, it might seem like the model performed poorly, however, upon inspection of the misclassified instances, we can see how similar each category is 
(probably because they share keywords or authors) mkaing it difficult for the model to accurately distinguis each category. 

### Packages used for this project include:
- Tensorflow
- Keras
- Numpy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- re
- os
- Opendatasets
<br/>

### Data
The [data](https://www.kaggle.com/datasets/rmisra/news-category-dataset?datasetId=32526&sortBy=voteCount) used for this project was gotten from Kaggle.

The dataset contains around 210k news headlines from 2012 to 2022 from HuffPost. This is one of the biggest news datasets and can serve as a benchmark for a variety of computational linguistic tasks.

The dataset has 6 features:

- category: category in which the article was published.
- headline: the headline of the news article.
- authors: list of authors who contributed to the article.
- link: link to the original news article.
- short_description: Abstract of the news article.
- date: publication date of the article.
- with our target (category) having 42 distinct values.

### Model Architecture
![image](https://github.com/Jeremyugo/News-Category-Classifier/assets/36512525/14a68736-b809-442a-9511-ee3f83bbf83c)


### Model predictions
![image](https://github.com/Jeremyugo/News-Category-Classifier/assets/36512525/f7bb790b-544a-4da5-8940-4df73e84b3cf)
