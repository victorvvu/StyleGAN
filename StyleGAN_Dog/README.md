# StyleGAN2 Dog Net
This dataset was taken from a paper from Khosla, and contains 20,000 images of dogs.

Here I utilize the architecture of StyleGAN2 to create (512x512) images of dogs. 


## 1. Summary 
##### Overview
The pitfall of GANs are that they require massive amounts of compute power to train, meaning they need stacks of GPUs to train. At a very high level, GANs are essentially 2 neural networks, one discriminator and one generator model, that are competing against each other. The discriminator produces fake images and is trying to fool the discriminator model in to believing that the images are real. 

This network improved on the pitfalls of StyleGAN1, where "water drops" can be seen on the images and did not allow users to control features. In addition, StyleGAN2 not only improves training time and performance, but it also produces extremely high quality images.

##### Training
The Nvidia team recommends training on 8-12 GPUs, however most of us do not have this type of hardware to do so. This means training on an Amazon EC2 instance will probably take a few days of constant training. Unfortunately for me, Amazon removed my free p2 instance, after leaving the model train for a whole day. So now I am training on Google Colab, which is much worse, since it automatically stops training after ~8 hours. 


## 2. Results

- still training on Colab

  
## 3. Data Description
Sample from dataset



![Sample2](https://github.com/victorvvu/Simple_CNGAN_Dogs/blob/main/dog_imgs/n02100236_2204.jpg?raw=true)


- 20,000 images of dogs
- 120 breeds
- labels include but not needed for this project

## 4. Road Map
- [x] Gather images and preprocess images
- [x] Train on Amazon EC2 Instance
- [x] Get my free P2 instance revoked 
- [ ] Train on Google Colab 
- [ ] Make application with generated images 
## 5. References

Aditya Khosla, Nityananda Jayadevaprakash, Bangpeng Yao and Li Fei-Fei. Novel dataset for Fine-Grained Image Categorization. First Workshop on Fine-Grained Visual Categorization (FGVC), IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2011.

http://vision.stanford.edu/aditya86/ImageNetDogs/

https://www.tensorflow.org/tutorials/generative/dcgan#setup
