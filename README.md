# Classifying fake news articles
## 1. Introduction
The goal of this report is to generate a deep learning model to determine the **probability** of an article containing false and misleading information. test with recurrent neural network

## 2. Initial Data Analysis
### 2.1 Data Sources
Dataset 1: https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset

From the first data set *Fake.csv* and *True.csv* were used. 

Dataset 2: http://web.eecs.umich.edu/~mihalcea/downloads.html#FakeNews

From the second data set all the .txt files in *celebrityDataset* and *fakeNewsDataset* were used.



### 2.2 Summary of datasets 
Both *Fake.csv* and *True.csv* contains 4 features, *title*, *text*, *subject* and data

*Fake.csv* contains 23481 observations and *True.csv* 21417 observations.

After combining the .txt files in the folders *celebrityDataset* and *fakeNewsDataset*, there were 490 fake news articles and 490 legitimate articles.

## 3. Dependencies and how to run the model on specific texts  
First create a folder named *data* and place it in the same directory as *fake_texts_classifier.ipynb*. Next download both datasets and extract them into the *data* folder (do not change the name of the folders).

To train the model simply run all cells in the notebook.

To test the model on any text call the *predict_text* function. A result closer to 1 indicates that the text is not trustworthy, whilst a result closer to 0 indicates that the text is legitimate.  

## 4. Overview of model - outline layers etc and why you used that 

## Results from model - validation , test accurancy graph outline that 