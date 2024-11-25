# Module 1 - Artificial Neural Network 
> **Instructor**: Emmanuel Asare (<ins>emmanuelasare@<i></i>ufl.edu</ins>) <br>
> **Co-author**: Silas Achidago (<ins>s.achidago@<i></i>ufl.edu</ins>)

# Neural Networks Overview
## Artificial Neural Networks (ANN)
**What is a neural network?**: **An Artificial Neural Network (ANN)** is a computational model inspired by the way biological neural networks in the brain process information. ANNs consist of layers of interconnected nodes (neurons) that transform input data into output predictions. <br>



## Structure
  - **Input Layer**: The input layer receives the raw data (e.g., satellite images or geographical data). Each neuron in this layer corresponds to one feature or variable in the data.
  - **Hidden Layers**: These are intermediate layers between input and output. They apply transformations to the data using weights and biases. The number of hidden layers and neurons per layer defines the complexity of the model. In simple ANNs, these layers are **fully connected** (dense), meaning each neuron in a layer is connected to every neuron in the next layer.
  - **Output Layer**: This layer produces the final prediction, which could be a class label (in classification tasks) or a continuous value (in regression tasks).

<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/ann.png">
</p>

- **Neuron**: A neuron (or node) is a fundamental unit in artificial neural networks (ANNs) that processes input data and produces output.

- **Activation Functions**: Activation functions play a crucial role in deep learning by introducing non-linearity into the neural network.


- **Forward and backward propagation**: The **forward** pass produces predictions based on the current weights and biases of the network. These predictions are then compared to the actual labels using a loss function, which calculates the error. **Backpropagation** is the process of calculating gradients for each weight and bias in the network and then updating them to minimize the error.

- **Loss Functions**: <br>
a. **Mean Squared Error (MSE)**: MSE calculates the average squared difference between predicted values (​ŷi) and actual values (yi).
<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/mse-function.png">
</p>

b. **Mean Absolute Error (MAE)**: MAE calculates the average absolute difference between predicted and actual values.
<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/mae-function.png">
</p>

c. **Binary Cross-Entropy (BCE)**: BCE measures the difference between actual and predicted probabilities in binary classification.
<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/bce-function.png">
</p>
    
d. **Categorical Cross-Entropy**: This is an extension of binary cross-entropy for multi-class classification.
