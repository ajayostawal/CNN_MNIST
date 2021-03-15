# CNN_MNIST

what is cnn?


convolution neural network working is similar to neural network , where input is multiplied with weights and add bias (z=x * w + b ) where each neuron store output of previous layer(z) and activation function.Activation function of neuron is input to next layer which get multiplied with w and add bias.

Similarly,
CNN image is input in form of array of matrix(ndarray) which get multiplied with filter(weights) and there can be multiple filters such as vertical,horizontal,diagonal,edges,etc which has strides=1,2 most of the time and padding = 0,1...(padding=0 id valid padding and p=1,2,3.. is called Same padding) and we get the output where matrix size is reduced and filter size increase as we move forward.where we perform multiple convolution and pooling layer and then flatten the matrix in 1 dimension which makes input to fully connected layer(Dense) .


for eg: image size:28 x 28, filter = (3 x 3), num_of_filter = 32 , output = 28 - 3 + 1 = 26(height) x 26(width) x 32(number of channels)=26 x 26 x 32 we get.
if image is greyscale then image only has depth =1 and RGB image depth = 3 .


CNN consist of 3 layers

1]convolution + RELU

2]MaxPooling

3]Fully connected layer + Softmax

Activation function RELU make the output in modified version of image so it is mostly used.


MaxPooling is reducing size of matrix and not reduce the size of filter .


Pooling layer output is given input to FC layer and FC  output is store in LOGITS gives input to softmax which transpose the output in from of probablity called as softmax transfromation.

