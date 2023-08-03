# Identifying-the-Bird-Species-by-their-Call-Using-Convolutional-Neural-Network
Convolutional neural networks and a deep learning technique are used in this project to identify different bird species based on their calls. The Xeno-Canto website, which collects animal sounds from all around the world, is where the bird cries were collected from. 600 audio recordings of 12 different bird species were chosen.

## Software
R Studio

## Package
`library(abind)`
`library(tidyr)`
`library(keras)`
`library(dplyr)`
`library(caret)`

## Getting Started
A 343 (time) x 256 (frequency) "image" of the bird call is created by preprocessing the audio inputs to create spectrograms for each 2-second window.

## Methods
Convolutional Neural Network (CNN)

## Key Findings
- In the binary classification model, the neural network with a basic topology performs better with a 96.7% accuracy rate and a 26-second computation time. 
- A complex structure for multi-class models requires a lot of processing (8 mins) and performs fairly with 71% accuracy.   
    - It has wrongly identified as a Western Meadowlark twice and a Red-winged Blackbird twice out of 20 Northern Flickers. There is a possibility that both birds may be present at the same moment, and the model will be able to tell which bird is making the loudest sound.
    - Additionally,recording an audio with numerous birds chirping simultaneously also affects the model accuracy. This model can be used to track bird migration counts, identify variables influencing bird migration, and conserve threatened seasonal bird species. 

## Results
The goal of this project was to distinguish the different bird species based on the pitch and tone of their calls, CNN uses audio recordings that have had less transmission loss to create spectrogram images. The accuracy of the Binary model was 96%, and the computation took 26 seconds. The accuracy of the multi-class model was 71%, and its computation took 499 seconds. In the future, the input files can be enhanced with data augmentation  to improve the model's performance and to experiment with other model parameters, however as we add more layers, the computational time will increase.	

## References:
- MayankMishra. Convolutional Neural Networks, Explained. Published in Towards Data science.
<https://towardsdatascience.com/convolutional-neural-networks-explained-9cc5188c4939>
- James, G., Witten, D., Hastie, T., & Tibshirani, R. (n.d.).An Introduction to Statistical Learning. Retrieved April 26, 2023, from https://www.statlearning.com/ 

