---
layout: post
title: "Urban Sound 8K"
date: 2019-05-22
excerpt: "Sound Classification."
tags: [sample post, readability, test]
comments: false
---

This was my first solo project. This is a problem of Multi-class Audio Classification. This dataset contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music. The classes are drawn from the urban sound taxonomy.
 This project involded Speech Processing, Feature Extraction, Deep Learning technique like Neural Nets, CNN.
 First we extract MFCC, Mel-spectogram features through a python library called librosa. LibROSA is a python package for music and audio analysis. It provides the building blocks necessary to create music information retrieval systems.
 
 # lading audio files 
 Using load method of librosa library, we can read audio files. It takes file path as input and returns an array having amplitude samples along with sampling rate of file.

Librosa library has many methods already build to extract features mentioned in resources which then returns another array of features. We can use various combinations of those features. This is something you can play around and try how and which features like mfcc, spectral features, energy etc affect the classification of audio.

For eg, in first stage you can extract only mfcc features and then build up a model and check the accuracy. Then try the same with other features. In order to further improve accuracy, you can also try to use more than one type of features and check the results.
![](https://miro.medium.com/max/768/1*MoiYQrW3Qaft6lfPQYbUbw.png)
# MFCC
Mel Frequency Cepstral Coefficents (MFCCs) are a feature widely used in automatic speech and speaker recognition. They were introduced by Davis and Mermelstein in the 1980’s, and have been state-of-the-art ever since. Prior to the introduction of MFCCs, Linear Prediction Coefficients (LPCs) and Linear Prediction Cepstral Coefficients (LPCCs) (click here for a tutorial on cepstrum and LPCCs) and were the main feature type for automatic speech recognition (ASR), especially with HMM classifiers. This page will go over the main aspects of MFCCs, why they make a good feature for ASR, and how to implement them.

# Using CNNs
This is a very classical way of sound classification as it is observed that similar type of sounds have similar spectrogram (read resource 3 to understand more about spectrogram). A spectrogram is a visual representation of the spectrum of frequencies of sound or other signal as they vary with time. And thus we can train a CNN network which takes these spectrogram images as input and using it tries to generalize patterns and hence classify them.
