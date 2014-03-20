<h1>Digit Recognizer for MNIST Data Set</h1>
In this project, I try different classification methods to recognize the digits in the MNIST data set.

<h2>MNIST Data Set</h2>
There are 60000 training samples and 10000 testing samples in the MNIST data set. 
Detailed description about this data set could be found via http://yann.lecun.com/exdb/mnist/index.html. 
<h2>Features</h2>
Each training sample and testing sample is represented by a 28x28 pixel image. 
In the data set, each sample is represented by 28x28=784 dimensional vector. I directly use this vector as the feature vector of each sample. 
<h2>Classification Methods</h2>
<ul>
<li>
KNN: accuracy 97.04%, running time &#8776 3hr
</li>
<li>
Linear kernel SVM: accuracy 93.98%, training time &#8776 10min, testing_time &#8776 3min
</li>
<li>
Polynomial kernel SVM with degree 2: accuracy 91.35%, training time &#8776 20min, testing_time &#8776 8min
</li>
<li>
Radial basis kernel SVM with default gamma: accuracy 94.46%, training time + testing time &#8776 20min
</li>
<li>
Artificial Neural Network with 1 hidden layer (784-300-10): <br>
100 iterations: accuracy 97.51%, training time + testing time &#8776 50min <br>
300 iterations: accuracy 97.56%, training time + testing time &#8776 2hr 30min
</li>
<li>
Convolutional Neural Network
</li>
</ul>

<h2>Usage</h2>
Since I use stanford's matlab function "loadMNISTImages" and "loadMNISTLabels" to load the data, you need to download theese two functions first. The link is as follows:
http://ufldl.stanford.edu/wiki/index.php/Using_the_MNIST_Dataset <br>

If you want to test a specific classification method of mine, you need to put loadMNISTImages.m, loadMNISTLabels.m, the data set and my code in the same directory. 
And then you just need to type the file name to run my code. I add detailed comments for my code, which should be useful if you want to modify my code. 


