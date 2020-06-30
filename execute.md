### Execute steps

0. Download the complete datasets from [1,2,3] or pick the reduced versions from [datasets](/datasets).
1. Run [01_dataset_combiner.ipynb](01_dataset_combiner.ipynb). Files *dataset_train.csv* and *dataset_test.csv*. (~ 3 min)
2. Run [02_pre_processer.ipynb](02_pre_processer.ipynb). Files *dataset_train_pp.csv* and *dataset_test_pp.csv* will be created. (~ 4 min)
3. Run one of the vectorizers:
    * [03_vectorizer_tfidf.ipynb](03_vectorizer_tfidf.ipynb) Define the vector length (300, 10000, 8000) in code (~ 1 min)
    * [03_vectorizer_word2vec_google.ipynb](03_vectorizer_word2vec_google.ipynb) Define the vector length (80, 115, 300) in code (~ 2 min)
    * [03_vectorizer_word2vec_news.ipynb](03_vectorizer_word2vec_news.ipynb) (~ 2 min) <br />
    Two file containing the vectorized dataset will be created, ex. *w2v_train_x_8000.npy*, *w2v_test_x_8000.npy* <br />
    Besides, for w2v notebooks, a vectorizer model file will be created, ex. *w2v_115.model*.
4. Run one of the cleassifiers:
    * [04_classifier_tfidf_300.ipynb](04_classifier_tfidf_300.ipynb) (~ 50 min)
    * [04_classifier_tfidf_1000.ipynb](04_classifier_tfidf_1000.ipynb) (~ 3h 20m)
    * [04_classifier_tfidf_8000.ipynb](04_classifier_tfidf_8000.ipynb) (~ 12 min)
    * [04_classifier_w2v_80.ipynb](04_classifier_w2v_80.ipynb) (~ 13 min)
    * [04_classifier_w2v_115.ipynb](04_classifier_w2v_115.ipynb) (~ 13 min)
    * [04_classifier_w2v_300.ipynb](04_classifier_w2v_300.ipynb) (~ 18 min)
    * [04_classifier_w2v_google.ipynb](04_classifier_w2v_google.ipynb) (~ 22 min) <br />
    Each of these notebooks
        * will train 3 classifiers (Naive-Bays, SVM, NN),
        * perform prediction on test set,
        * plot confusion matrix,
        * and save model file of the NN classifier, ex. *nn_tfidf_8000.h5*.
  5. To do inference step, copy the classifier model file and if needed, the vectorizer model file in [inference](/inference) folder. Then run one of the inference notebooks. Each notebook contain 25 piece of news article picked from [DW English](dw.com). The inference results will be printed.
