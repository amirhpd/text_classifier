# Implementation and Evaluation of Text Classifiers

![alt text](https://github.com/amirhpd/text_classifier/blob/master/graphs/cls1.png "Classifier")

## Abstract:
This project aims to implement and compare different types of text classifiers on the news text data. A dataset of labeled text will be used to train the model. The evaluation of each method will be done using the test dataset. A comparison between the performance of the classifiers will be delivered.

## Steps:
1. **Dataset Collection:** A combination of three datasets of news articles will be used:
    * AG's News Topic Classification Dataset [1]: <br />
    Contains 120,000 train samples and 7,600 test samples of news texts, and labeled in 4 categories of World, Sports, Business, Science.
    * COVID-19 News Articles Open Research Dataset [2]: <br />
    Contains more than 5,000 news test items about COVID-19.
    * Covid-19 Public Media Dataset by Anacode [3]:  <br />
    Contains over 50,000 text articles about COVID-19, from different online sources. Items of news articles will be selected for this project.

    The combination of the mentioned dataset will provide a larger dataset with 5 labels:  **World, Sports, Business, Science, and Corona**.

2. **Text pre-processing:** The following operations will be done on the text data:
    * Tokenization
    * Punctuation and number removal
    * Stop word removal
    * Convert to lower-case
    * Lemmatization

<br />

3. **Text Vectorization:** Text data will be converted to vectors. Two different NLP techniques will be applied and the results of each will be compared:
    * TF-IDF
    * Word2Vec

<br />

4. **Classification:** Different supervised classification techniques will be applied and results will be converted. Besides, some NLP-based techniques will be tried:
    * Naive Bays classifier
    * SVM
    * Neural networks

<br />

5. **Evaluation:** Results of all different methods will be compared. A benchmark based on the parameters of train/test accuracy, memory usage, and processing time will be delivered.

<br />

Follow [this](execute.md) guide to execute the files.<br />
Here is the [Slide set](Implementation%20and%20Evaluation%20of%20Text%20Classifiers.pdf) (subject to copyright)

<br />
<br />
<br />

\[1]: https://www.kaggle.com/amananandrai/ag-news-classification-dataset <br />
\[2]: https://www.kaggle.com/ryanxjhan/cbc-news-coronavirus-articles-march-26 <br />
\[3]: https://www.kaggle.com/jannalipenkova/covid19-public-media-dataset <br />
