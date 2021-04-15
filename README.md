# House Price Prediction 

## A. PROJECT SUMMARY

**Project Title:** House Price Prediction

**Team Members:** 
- Siew Chung Seng 
- Cecilia Chong Ching Nee
- Vishan Menan A/L Balakrishnan
- Muhammad Putra Alif bin Ismail


- [ ] **Objectives:**
- To predict house prices



##  B. ABSTRACT 

The topic of fake news detection on social media has recently attracted tremendous attention. The basic countermeasure of comparing websites against a list of labeled fake news sources is inflexible, and so a machine learning approach is desirable. Our project aims to use Natural Language Processing to detect fake news directly, based on the text content of news articles.


![Coding](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/09/python-project-detecting-fake-news.jpg)
Figure 1 Fake news detection


## C.  DATASET
rain.csv: A full training dataset with the following attributes:

- id: unique id for a news article
- title: the title of a news article
- author: author of the news article
- text: the text of the article; could be incomplete
- label: a label that marks the article as potentially unreliable
- 1: unreliable
- 0: reliable
- test.csv: A testing training dataset with all the same attributes at train.csv without the label.



## D.   PROJECT STRUCTURE

The following directory is our structure of our project:
- .
- |
- |--- datasets
- |------- train.csv
- |------- test.csv
- | images
- |------ svm-cm.png
- |------ naive-bayes-cm.png
- |------ neural-net-tf.png
- |------ neural-net-keras.png
- |------ lstm-cm.png
- +-- *.py


## E   TRAINING THE FAKE NEWS DETECTION

We are now ready to train our face mask detector using Keras, TensorFlow, and Deep Learning.

From there, open up a terminal, and execute the following command:

- $ python train_fake_news_detector.py --dataset dataset
- [INFO] loading images...
- [INFO] compiling model...
- [INFO] training head...
- Train for 34 steps, validate on 276 samples
- Epoch 1/20
- 34/34 [==============================] - 30s 885ms/step - loss: 0.6431 - accuracy: 0.6676 - val_loss: 0.3696 - val_accuracy: 0.8242
- Epoch 2/20
- 34/34 [==============================] - 29s 853ms/step - loss: 0.3507 - accuracy: 0.8567 - val_loss: 0.1964 - val_accuracy: 0.9375
- Epoch 3/20
- 34/34 [==============================] - 27s 800ms/step - loss: 0.2792 - accuracy: 0.8820 - val_loss: 0.1383 - val_accuracy: 0.9531
- Epoch 4/20
- 34/34 [==============================] - 28s 814ms/step - loss: 0.2196 - accuracy: 0.9148 - val_loss: 0.1306 - val_accuracy: 0.9492
- Epoch 5/20
- 34/34 [==============================] - 27s 792ms/step - loss: 0.2006 - accuracy: 0.9213 - val_loss: 0.0863 - val_accuracy: 0.9688
- ...
- Epoch 16/20
- 34/34 [==============================] - 27s 801ms/step - loss: 0.0767 - accuracy: 0.9766 - val_loss: 0.0291 - val_accuracy: 0.9922
- Epoch 17/20
- 34/34 [==============================] - 27s 795ms/step - loss: 0.1042 - accuracy: 0.9616 - val_loss: 0.0243 - val_accuracy: 1.0000
- Epoch 18/20
- 34/34 [==============================] - 27s 796ms/step - loss: 0.0804 - accuracy: 0.9672 - val_loss: 0.0244 - val_accuracy: 0.9961
- Epoch 19/20
- 34/34 [==============================] - 27s 793ms/step - loss: 0.0836 - accuracy: 0.9710 - val_loss: 0.0440 - val_accuracy: 0.9883
- Epoch 20/20
- 34/34 [==============================] - 28s 838ms/step - loss: 0.0717 - accuracy: 0.9710 - val_loss: 0.0270 - val_accuracy: 0.9922
- [INFO] evaluating network...

|    Model   | accuracy| 
|-----------------|-------|
|Naive Bayes|	72.94%|
|SVM|	88.42%|
|Neural Network with TF|	81.42%|
|Neural Network with Keras|	92.62%|
|LSTM|	94.53%|


![Figure 4](https://www.pyimagesearch.com/wp-content/uploads/2020/04/face_mask_detector_plot.png)

Figure 4: Fake News Dectector training accuracy
As you can see, we are obtaining ~99% accuracy on our test set.

Looking at Figure 4, we can see there are little signs of overfitting, with the validation loss lower than the training loss. 

Given these results, we are hopeful that our model will generalize well to images outside our training and testing set.


## F.  RESULT AND CONCLUSION

Fake News Detection Tutorial video



[![Figure5](https://i.ytimg.com/vi/GS_ylghUtLQ/hqdefault.jpg?sqp=-oaymwEbCKgBEF5IVfKriqkDDggBFQAAiEIYAXABwAEG\u0026rs=AOn4CLC0tdcKDsZpSjcb3cxSlaJEIo7mLA)](https://www.youtube.com/watch?v=GS_ylghUtLQ&ab_channel=MachineLearningHub)

Figure 5: Fake News Detection tutorial





## G.   PROJECT PRESENTATION 





