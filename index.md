---
layout: default
---

I am **Rama**, a Data Scientist from Mumbai, India. I have created this page to list out some of my experiments in Natural Language Processing and Computer Vision.

### Natural Language Processing

Worked on projects on Text Classification and Sentiment Analysis.

1. **"Real or NOT" : NLP to Identify Public Emergency Related Tweets** [[code](https://github.com/raamav/Text-Classification)] : Twitter has become an important communication channel in times of emergency. Its vital to be able to identify the Tweets that are about real Emergencies. However, it’s not always easy to do so.
   * **Potential Applications** These algorithms can be used by Governments to better manage the responses to Public Emergencies
   * **Data**: The dataset comprises 7500+ tweets which cover a wide set of public emergencies like Natural Disasters
   * **Approach**: Used a neural net with Bi-Directional LSTMs to extract the sentiment
   * **Results**: The best performing model had an accuracy of 83% on the test set

2. **Sentiment Analysis on Full-Length Movie Reviews (IMDB)** [[code](https://github.com/raamav/Sentiment-Analysis-UserReviews/blob/master/IMDB_Reviews_DeepLearning_(v2).ipynb)] : IMDB Reviews is one of the best known publically available datasets for sentiment analysis. The reviews in the dataset are selected across movies and genres.
   * **Data**: The dataset comprises 50,000 'full-length' reviews. Most of these reviews are several paragraphs long
   * **Approach**: 
        * From an architectural standpoint, I used a three-layer Bidirectional LSTM network followed by a set of three Dense layers. Incorporated `Recurrent Dropout` which greatly improved the validation accuracy
        * Used Pre-Trained Word Embeddings to further improve the classification accuracy. Used the 100-dimensional `GloVe` embedding as an input to the deep network
        * Employed innovative approaches of text-preprocessing, such as expanding out word contractions *(don't >> do not)* and possessives *(people's >> people s)* 
   * **Results**: The best performing model had an accuracy of 86% on the test set


<BR>
  
### Computer Vision

Worked on projects on Image Classification and Image Color Segmentation.

1. **Image Color Segmentation** [[code](https://github.com/raamav/Image-Color-Segmentation)]: Segmenting images by their color and Detecting the Top 3 colors in a given image along with their relative densities (% area). 
   * **Applications**: Potential applications in e-commerce *(automatically filling out the color information for a catalog)*. The algorithm can also be used in tandem with object detection algorithms to specify the color of the object detected *(e.g. a red car)*
   * **Approach**: 
     * The application is based on the K-Means clustering algorithm. An improved version of the K-Means algorithm, K-Means++ is used. This algorithm features a better way of initializing the weights which results in a more optimal solution while taking less time to execute
     * The RGB values of the colors are used to generate the names of the colors (the webcolors library helps to do this)
   
2. **Interpreting Hand Gestures** [[code](https://github.com/raamav/Image-Classification/blob/master/Interpreting_Hand_Gestures_(Signs).ipynb)] : This dataset comprises images of hand gestures that indicate numerals from *zero to five*. 
   * **Potential Applications**: This analysis is a step towards helping computers interpret human-sign language.
   * **Data**: The dataset comprises 1080 training images *(less than 200 images per class)* and there are 120 images in the test set. 
   * **Approach**: 
        * Implemented architecture similar to `AlexNet` which resulted in a 94% accuracy in the test set 
        * Created a `Resnet - 50` architecture from scratch, which unsurprisingly did not work well (The number of images is way too less) 
        * Used Transfer Learning using (pre-trained) weights from the `DenseNet 121` model. Post an initial round of training (30 epochs), fine-tuned the model by unfreezing all the weights. The resulting model performed exceedingly well with 96% accuracy on the test set
   * **Results**: Got the best results from Transfer Learning. The best model had a 96% accuracy on the test set.

<BR>

### Other Projects

1. **Forecasting Atmospheric Co2** [[code](https://github.com/raamav/Time-Series-Analysis/blob/master/6.%20Forecasting_Atmospheric_CO2.ipynb)]: The Mauna Loa observatory in Hawaii, USA has been recording Co2 concentrations on a monthly basis from the late 1950s. The goal is to forecast the monthly average CO2 concentration for 2018 and 2019 given the data from 1958 to 2017
   * **Approach**: Used Holt-Winter's method and Seasonal ARIMA based models both of which performed very well
   * **Results**: Got near-perfect results from the approaches mentioned. 

<BR>

### Degrees 

| Degree       | University        | Year |
|:-------------|:------------------|:------|
| MBA          | NMIMS, Mumbai     | 2009  |
| BE (Telecom.)| VTU, Belgaum      | 2005  |


<BR>

### Coursework

All of these courses are of 12 - 16 weeks in duration and are adapted from the courses that are offered in the respective universities. 

1. **Deep Learning Specialization**, offered by Deeplearning.ai (2020)
2. **Data Structures and Algorithms Specialization**, offered by University of California San Diego via Coursera.org (2020)
3. **Machine Learning**, offered by Stanford Online via Coursera.org (2019)
4. **Discrete Math Specialization**, University of California San Diego via Coursera.org (2020)
5. **Introduction to Computer Science and Programming using Python**, offered by MIT Online via edX.org (2019)
6. **Computer Architecture**, offered by Princeton University via Coursera.org (2019)
7. **The Analytics Edge**, offered by MIT Online via edX.org (2015)
8. **Data Analysis and Statistical Inference**, offered by Duke University Online via coursera.org (2014)


* * *
