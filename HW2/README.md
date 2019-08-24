## q1.ipynb

**Description:** Implementation of 4-layer neural network from scratch. The visualization of the final calssification region is implemented and analysed. A pdf version of the report is also in the folder.

**Dataset:** XOR with 4 data points. Certain noise is added for further analysis of the NN generalization ability.

**model architecture:** 1 input layer, 2 hidden layer both with 4 neurons and 1 output layer. The input layer has 2 neurons because each point has 2 values (x and y). The output layer has 2 neurons because the label is converted to one hot representation. Index 0 represent class 1 and index 1 represents class -1. The loss function I choose are tanh except the output layer which is sigmoid since the output layer should be the probability of each label. I set the hidden layer in this form after seceral experiments and this one has a relatively better classification region when visualizing it. The loss function is cross-entropy loss. It measures the performance of a classification model whose output is a probability value between 0 and 1. Cross-entropy loss increases as the predicted probability diverges from the actual label.

**Used packages:** numpy, matplotlib, seaborn

## q2.ipynb
**Description:** Implementation of convolutional neural network using tensorflow on CIFAR-10 dataset. Report also included.

**model architecture:**  
**Input:** 32\*32\*3   
**Convolution layer 1:**  
Kernel size: 5\*5\*3  
Activation function: relu  
**Normalization and Pooling Layer 1:** [2\*2]  
**Convolution layer 2:**  
Kernel size: 5*5*64  
Activation function: relu  
**Normalization and Pooling Layer 1:** [2\*2]  
**Fully connected layer:**  
Neurons: 1024  
**Output layer:**  
Neurons: 10  
Activation function: softmax  
Loss function: cross-entropy loss  

**Used packages:** tensorflow, numpy, matplotlib, seaborn, amth, pandas
