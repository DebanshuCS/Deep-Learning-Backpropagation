# Deep-Learning-Backpropagation

Backpropagation is usually the hardest (most mathematical) part in deep learning. It is the algorithm widely used for training feedforward neural networks. 

### Dataset
Let’s get the dataset we will work on. The following code will load a “flower” 2-class dataset into variables X and Y.

```
X, Y = load_planar_dataset()
```
You can visualize the dataset with the help of matplotlib. The data will be like a “flower” with red and blue petals.

**We need to build a model to fit this data.**

First we need to make sense of the data which we have. We need to make use of Numpy

We have,

**a numpy-array (matrix) X that contains your features (x1, x2)**
**a numpy-array (vector) Y that contains your labels (red:0, blue:1)**,

We need to make use of “Shape of the array”.

<img width="487" alt="Screenshot 2023-01-07 at 9 58 42 PM" src="https://user-images.githubusercontent.com/118846871/211160852-fdddf920-ced6-42a4-af43-3c7409ecf17d.png">

Neural Networks learn through iterative tuning of parameters (weights and biases) during the training stage. At the start, parameters are initialized by randomly generated weights, and the biases are set to zero.
This is followed by a forward pass of the data through the network to get model output. Lastly, back-propagation is conducted. 
The model training process typically entails several iterations of a forward pass, back-propagation, and parameters update.

### This Notebook:

 - Implement a 2-class classification neural network with a single hidden layer
 - Use units with a non-linear activation function, such as tanh 
 - Compute the cross entropy loss 
 - Implement forward and backward propagation.
 
### Cost iteration Diagram:

<img width="612" alt="Screenshot 2023-01-07 at 9 57 41 PM" src="https://user-images.githubusercontent.com/118846871/211161318-5480b653-f58e-478e-ba5d-0202bb65bf1d.png">

 
 **Interpretation**:
 - The larger models (with more hidden units) are able to fit the training set better, until eventually the largest models overfit the data. 
 - The best hidden layer size seems to be around n_h = 5. Indeed, a value around here seems to  fits the data well without also incurring noticable overfitting.
 - You will also learn later about regularization, which lets you use very large models (such as n_h = 50) without much overfitting. 

**Optional questions**:
 
 **Note**: Remember to submit the assignment but clicking the blue "Submit Assignment" button at the upper-right. 
 
 Some optional/ungraded questions that you can explore if you wish: 
 - What happens when you change the tanh activation for a sigmoid activation or a ReLU activation?
 - Play with the learning_rate. What happens?
 - What if we change the dataset? (See part 5 below!)


 **Target:**
 - Build a complete neural network with a hidden layer
 - Make a good use of a non-linear unit
 - Implemented forward propagation and backpropagation, and trained a neural network
 - See the impact of varying the hidden layer size, including overfitting.



 
 
