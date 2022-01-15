## LeNet5
LeNet is a convolutional neural network structure proposed by Yann LeCun et al. in 1989. It was one of the earliest convolutional neural networks and promoted the development of deep learning.

### Architecture
<img src="https://miro.medium.com/max/700/1*lvvWF48t7cyRWqct13eU0w.jpeg">

<br>

<> | Layer | #Filters / Type | Filter size | Stride | Size | Activation Function
--- | --- | --- | --- | --- | --- | ---
1 | Input | | | | 32x32x1 
2 | Conv2d | 6 | 5x5 | 1 | 28x28x6 | tanh
3 | AveragePooling2d | avg | 2x2 | 2 | 14x14x6 |
4 | Conv2d | 16 | 5x5 | 1 | 10x10x16 | tanh
5 | AveragePooling2d | avg | 2x2 | 2 | 5x5x16 |
6 | Conv2d | 120 | 5x5 | 1 | 120 | tanh
7 | Linear | |  |  | 120 | tanh
8 | Linear | |  |  | 84 | tanh
8 | Final Linear | |  |  | 10 | softmax

<br>

### References
- [Wikipedia](https://en.wikipedia.org/wiki/LeNet)
- [Medium](https://medium.com/analytics-vidhya/lenet-with-tensorflow-a35da0d503df)