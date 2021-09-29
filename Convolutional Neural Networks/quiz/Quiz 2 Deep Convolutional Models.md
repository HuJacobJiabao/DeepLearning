## Deep Convolutional Models
1. Which of the following do you typically see in a ConvNet? (Check all that apply.)
   >* Multiple CONV layers followed by a POOL layer
   >* FC layers in the last few layers
2. In order to be able to build very deep networks, we usually only use pooling layers to downsize the height/width of the activation volumes while convolutions are used with “valid” padding. Otherwise, we would downsize the input of the model too quickly.
   >* False
3. Training a deeper network (for example, adding additional layers to the network) allows the network to fit more complex functions and thus almost always results in lower training error. For this question, assume we’re referring to “plain” networks. 
   >* False
4. The following equation captures the computation in a ResNet block. What goes into the two blanks above? 
   $a ^{[l+2]} = g(W^{[l+2]}g(W^{[l+1]}a^{[l]}+b^{[l+1]}) + b^{[l+2]} + \underline{\qquad \qquad} ) + \underline{\qquad \qquad}$
   >* $a^{[l]}$ and 0, respectively
5. Which ones of the following statements on Residual Networks are true? (Check all that apply.)
   >* The skip-connection makes it easy for the network to learn and identity mapping between the input and the output within the ResNet block.
   >* Using a skip-connection helps the gradient to backpropagate and thus helps you to train deeper networks.
6. Suppose you have an input volume of dimension $n_H \times n_W \times n_C$. Which of the following statements you agree with? (Assume that “1x1 convolutional layer” below always uses a stride of 1 and no padding.)
   >* You can use a 2D pooling layer to reduce $n_H$, $n_W$, but not $n_C$.
   >* You can use a 1×1 convolutional layer to reduce $n_C$ but not $n_H$. $n_W$
7. Which ones of the following statements on Inception Networks are true? (Check all that apply.)
   >* A single inception block allows the network to use a combination of 1 ×1, 3×3, 5×5 convolutions and pooling.
   >* Inception blocks usually use 1×1 convolutions to reduce the input data volume's size before applying 3×3 and 5×5 convolutions.
8. Which of the following are common reasons for using open-source implementations of ConvNets (both the model and/or weights)? Check all that apply. 
   >* Parameters trained for one computer vision task are often useful as pretraining for other computer vision tasks.
   >* It is a convenient way to get working with an implementation of a complex ConvNet architechture.
9.  In Depthwise Separable Convolution you:
    >* You convolve the input image with $n_c$ number of $n_f × n_f$ filters($n_c$ *is the number of color channels of the input image*).
    >* The final output is of the dimension $n_{out} × n_{out} × n^\prime_c$(*where $n^\prime_c$ is the number of filters used in the previous convolution step*).
    >* For the "Depthwise" computations each filter convolves with only one corresponding color channel of the input image.
    >* Perform two steps of convolution.
10. Fill in the missing dimensions shown in the image below (*marked* *W, Y, Z*).
   > <div>
   > <img src=1632849702(1).jpg# width=100% />
   > </div>
   
   >* W = 5, Y = 30, Z = 20
   
