# DLND_Face-Generation-P5
**Jianguo Zhang, May 22, 2017**

This project uses generative adversarial networks(GAN) to generate new images of faces using [Large-scale CelebFaces Attributes (CelebA) Dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html). 
 

The Mnist Dataset is a database of handwritten digits, which includes a training set of 60,000 examples, and a test set of 10,000 examples. The CelebA dataset contains over 200,000 celebrity images with annotations.

Since the celebA dataset is much complex, we first `test` and `tune` our neural network on the [Mnist Dataset](http://yann.lecun.com/exdb/mnist/). Then `use` it on the CelebA dataset to generate face images. 

Our network is `a little` similiar with [Deep Convolutional GANs(DCGAN)](https://arxiv.org/pdf/1511.06434.pdf), The DCGAN architecture was first explored last year and has seen impressive results in generating new images, we modify its architecture in this project. 

The project uses [TensorFlow==1.0.0](https://www.tensorflow.org/)  and [python==3.6](https://www.python.org/downloads/release/python-361/) and runs on [AWS EC2 g2.2xlarge](https://aws.amazon.com/ec2/) GPU device. Please make sure that you install all depencies before run the project, the [requirements](https://github.com/JianguoZhang1994/DNLD_Tv_Script_Generation-P3/blob/master/requirements.txt) incldues minimum requirements of depencies. You should also have a GPU device to accelerate training process. 

When you run our project. Make sure the loss of the generator is lower than the loss of the discriminator or close to 0.

### Explore dataset:

<div align=center>
<img src="./demo/Dataset_Mnist.png?raw=true" width="330" height="300" />
<img src="./demo/Dataset_CelebA.png?raw=true" width="330" height="300" />
</div>


### Results:

**First**, we test and tune our neural network on Mnist Dataset. Following are the the generated results.

<div align=center>
<img src="./demo/Result_Mnist.png?raw=true" width="345" height="300" />
<img src="./demo/Image_Mnist.png?raw=true" width="350" height="300" />
</div>

**Then**, we run our neural network on the large scale CelebA Dataset. Following are the generated results.

<div align=center>
<img src="./demo/Result_CelebA.png?raw=true" width="345" height="300" />
<img src="./demo/Image_CelebA.png?raw=true" width="350" height="300" />
</div>

