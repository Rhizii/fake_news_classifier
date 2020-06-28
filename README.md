# Classifying fake news articles
## 1. Introduction
The goal of this report is to generate a deep learning model to determine the **probability** of an article containing false and misleading information. The model uses *dense* hidden layers to learn the dependencies between words and explore certain characteristics of fake news articles. 

This model could be used as the the backend of a mobile application which allows users to highlight text on any app (eg WhatsApp or Facebook) to identify if a message/text is untrustworthy. This would protect users from being mislead by false information.

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
First create a folder named *data* and place it in the same directory as *final_Hrishikesh-Masurkar.ipynb*. Next download both datasets and extract them into the *data* folder (do not change the name of the folders).

To train the model simply run all cells in the notebook. 

To test the model on any text call the *predict_text* function. A result closer to 1 indicates that the text is not trustworthy, whilst a result closer to 0 indicates that the text is legitimate.  


## 4. Results from model 
Overall, the validation and test loss graph show that that validation loss is consistently lower than the training loss also decreases are a similar rate over the epochs.

Futhermore, the model attains an overall accuracy of ~96% when evaluate on the testing set.

## 5. Conclusion
The model has shown promising results and has accurately identified articles and messages as untrustworthy. However, the neural network should be trained on new and current datasets to ensure it is kept up to date. 

