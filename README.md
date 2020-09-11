# Neural_Networks_from_Scratch
Creating a Neural Network step by step without using any ML / DL library

- Initialize the parameters for a two-layer network and for an L-layer neural network.
- Implement the forward propagation module (shown in purple in the figure below).
     - LINEAR part of a layer's forward propagation step (resulting in Z[l]).
     - ACTIVATION function on Z[l] (relu/sigmoid).
     - Combine the previous two steps into a new [LINEAR->ACTIVATION] forward function. calculating g(Z[l])
     - Stack the [LINEAR->RELU] forward function L-1 time (for layers 1 through L-1) and add a [LINEAR->SIGMOID] at the end (for the final layer L). This gives you a new L_model_forward function.
- Compute the loss.
- Implement the backward propagation module (denoted in red in the figure below).
    - LINEAR part of a layer's backward propagation step calculating ( dA_prev, dW, db)
    - dZ[l] after ACTIVATION function (relu_backward/sigmoid_backward) 
    - Combine the previous two steps into a new [LINEAR->ACTIVATION] backward function. calculating new ( dA_prev, dW, db)
    - Stack [LINEAR->RELU] backward L-1 times and add [LINEAR->SIGMOID] backward in a new L_model_backward function
- Finally update the parameters.

<img src="images/finaloutline.png" style="width:800px;height:500px;">

 
