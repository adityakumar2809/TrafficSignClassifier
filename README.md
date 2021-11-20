# TrafficSignClassifier

## Introduction
With the advancement of Computer Vision technologies, it is extremely important for automobile industries to keep up with the pace and introduce new and revolutionary features in their designs. One such feature that was recently popularised by Honda was detection of traffic signs and their corresponding recognition. The ultimate aim of the project is not only to notify user in case he or she has missed any traffic sign but also, in recent future, implement enforcement technologies to ensure that the traffic safety rules are thoroughly implemented.

<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/speed_limiter_dashboard.jpg" />

## Dataset Used
The dataset we’ll be using to train our own custom traffic sign classifier is the German Traffic Sign Recognition Benchmark (GTSRB).

<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/dataset.jpg" />

The GTSRB dataset consists of 43 traffic sign classes and nearly 50,000 images.
A sample of the dataset can be seen in the given figure — here the traffic signs have been pre-cropped for use, implying that the dataset annotators/creators have manually labeled the signs in the images and extracted the traffic sign Region of Interest (ROI), thereby simplifying the project.

There are a number of challenges in the GTSRB dataset, the first being that images are low resolution, and worse, have poor contrast (as seen in Figure 2 above). These images are pixelated, and in some cases, it’s extremely challenging, if not impossible, for the human eye and brain to recognize the sign.

The second challenge with the dataset is handling class skew:

<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/DistributionOfImagesOverClassNumber.png" />

The top class (Speed limit 50km/h) has over 2,000 examples while the least represented class (Speed limit 20km/h) has under 200 examples — that’s an order of magnitude difference

## Methodology

<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/recognition_architecture.png"/>

Here is a sample of how augmented images look like after the processing
<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/AugmentedImages.png" />

## Training Phase

<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/AccuracyVSEpoch.png" />
<img src="https://github.com/adityakumar2809/TrafficSignClassifier/blob/master/images/LossVSEpoch.png" />

