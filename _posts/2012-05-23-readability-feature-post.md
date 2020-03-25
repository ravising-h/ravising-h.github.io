---
layout: post
title: "Assist Me"
date: 2019-10-23
excerpt: "Image Caption, Face Recognition, Image OCR, Text-to-Speech"
tags: [Face Recognition, OCR, RNN, image, feature]
comments: false
---
This is a web app developed for Blind people to make them feel their surroundings. In this app we brougth technologies like Face Recognition, Image OCR, Image Caption under a umbrella. It has text to speech which narrates all the scene to user.
This could easily installed on the sticks of Blind people. 
# Image Caption

Caption generation is a challenging artificial intelligence problem where a textual description must be generated for a given photograph.

It requires both methods from computer vision to understand the content of the image and a language model from the field of natural language processing to turn the understanding of the image into words in the right order. Recently, deep learning methods have achieved state-of-the-art results on examples of this problem.
![](https://github.com/ravising-h/Image-Caption/blob/master/Image%20Caption.png.jpeg)
* Photo Feature Extractor. This is a 16-layer VGG model pre-trained on the ImageNet dataset. We have pre-processed the photos with the VGG model (without the output layer) and will use the extracted features predicted by this model as input.
* Sequence Processor. This is a word embedding layer for handling the text input, followed by a Long Short-Term Memory (LSTM) recurrent neural network layer.
* Decoder (for lack of a better name). Both the feature extractor and sequence processor output a fixed-length vector. These are merged together and processed by a Dense layer to make a final prediction.
It helps user to identify what is happening arround it.

# Face Recognition
Recognize and manipulate faces from Python or from the command line with the world's simplest face recognition library.

Built using dlib's state-of-the-art face recognition built with deep learning. The model has an accuracy of 99.38% on the Labeled Faces in the Wild benchmark.
This could help blind people in recognizing who is standing in front of them.

# Image OCR

Optical character recognition or optical character reader is the electronic or mechanical conversion of images of typed, handwritten or printed text into machine-encoded text, whether from a scanned document, a photo of a document, a scene-photo or from subtitle text superimposed on an image.
 It will help them to identify traffic signal, Resturant menu and various sign.
