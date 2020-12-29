# Mask_Detection

This is my final project of Lighthouse Labs. 

## About
The model is a mask detection model. I used Convolutional Nueral Networks (CNN) to accomplish it. The data preprocessing and training took quite a bit of long time. I trained the model using different `layers` and `activation function`, and it took me 5 training to rwach the accuracy of 96.625%. At the end, I converted the model to a `CoreML` file which I then ised it in my iOS application-will release soon. 

## Dataset 
During my research for a dataset, I found many of them in Kaggle. However, there was one with 7553 images with two classes **with_mask** and **without_mask**. You can find the dataset [here](https://www.kaggle.com/omkargurav/face-mask-dataset).

## Demo
<img src="mask_test.gif" width="30%" height="60%"/>

## Challenges / What I learnt
1. It was my first time searching a dataset and doing all the preprocessing. In class, our data were mostly same size images and were very edited. However, I spent some amount of time to learn how to edit my dataset for training. 
2. Converting to `CoreML` took a lot of time but I could finally learn it.

## Further imporvement
1. My model doesn't recognize faces but knows when a mask is there on face or not. I am planning to train my model on `YOLO`'s Darkent so that it doesn't say no mask when there isn't a face.
2. Conversion to `CoreML` make the file too large. I would like to find a way to make the size smaller so that it can use less RAM on an iOS device. 
3. I found a dataset that had one additional class of **not_properly_worn**. However, it had very fewer images. I am planning to optimize that dataset or create/find a new one so that my model can say when a person is not wearing their mask properly.
