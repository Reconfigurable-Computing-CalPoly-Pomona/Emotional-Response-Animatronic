# Low-Cost Embedded Animatronic, Emotion Detection

Senior Project 2019-20

Project repository for Dominic Holloman, Kevin Worsley

* Files (Neural Network):
  * cnn-model-train.py : Training file for a convolutional neural network, training on the fer2013 dataset
  * dataset-load.py : Algorithm to take fer2013.csv and turn it into useful training format
  * image-inference.py : Runs a webcam object and performs inference with the model over its stream
  * keras-converter.py : Converts standard Tensorflow model format to TFLite for embedded device
  * pi-inference.py : Script for image collection and inference that runs on the Pi Zero W
  
* Files (Microcontrollers):
  * PIC18F4321_MainCode.C : This is the code from the presetation for the main microcontroller.
  * PIC12F1822_AudioCode.C : This is the code from the presetation for the microcontroller responsible for audio generation.
  
Presentation Link: https://youtu.be/V8JK8axZZhU
  
## Model information

The model is a Convolutional Neural Network, trained on the fer2013 emotion dataset (3995 examples per emotion). The network passes information through a variety of convolutional modules, before being flattened and loaded into a decreasing net of densely-connected layers. The input data is augmented to improve its accuracy in a real world environment. 


Supervising Professor:

- Mohamed El-Hadedy: Assistant Professor, Electrical and Computer Engineering department, College of Engineering, California State Polytechnic University, Pomona.

Collaborators:

1. Wen-Mei Hwu: Director of Center for Cognitive Computing Systems Research and Walter J. Sanders III-AMD Endowed Chair Professor in Elecrical and Computer Engineering at UIUC

2. Jinjun Xiong: Director of Center for Cognitive Computing Systems Research and Adjunct Research Professor at UIUC
Electrical and Computer Engineering

California Polytechnic University, Pomona
