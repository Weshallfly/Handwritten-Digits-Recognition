In this project, I have implemented a Feedforward Neural Network using TensorFlow and Keras to train a model  that recognizes handwritten digits.Following this, I tuned the hyperparameters of this model a bit and achieved higher accuracy. 

### Handwritten-Digits-Recognition
Handwritten digit recognition is the process to provide the ability to machines to recognize human handwritten digits.

### DATA
The MNIST Handwritten Digit Recognition Dataset contains 60,000 training and 10,000 testing labelled handwritten digit pictures. Each picture is 28 pixels in height and 28 pixels wide, for a total of 784 (28×28) pixels. Each pixel has a single pixel value associated with it.

## Steps in brief
Starting with some **EDA** in normalised data
Then starting with a simple **Feedforward Neural Network** with 2 hidden dense layers

### Hyperparametric Tuning
I have to find the best possible combination of hyperparameters in such a way that model is neither overfit nor underfit and giving a higher accuracy.

Model have many hypreparameters  
1.No of Layers  
2.No of units in different layers  
3.Activation function  
4.Epochs i.e. No of steps taken by Gradient decsent to reach minimum of cost function

To achieve a better accuracy I tried many things listed down,most of the thingd doesn't worked.This is may be because the type of data.

(1) I had tried different combinations of no, of layer,units and epochs but this didn't helped much.

(2) I tried to average the predictions of many different model but this also didn't helped.

(3) I tried to fit model on transformed data between 0 and 1. But this also didn't increased the accuracy.

(4) **Data Augmentating**
Analysing misclassified examples:Checked if particular digit is generating significantly more error than other digits.Algorithm can be confuse between same looking digits like 6,8 and 9. Then we can increase algorithm attention to them by **Augmentating** more data of them by modifying existing examples.

To achieve this, I just doubled each example with target variable 9 and 5.But this doesn,t helped much.So, I stopped working in this direction.
