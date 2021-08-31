# Attacking Neural Networks to Force Misclassifications

![Attack in Action](https://github.com/vs1720/Neural_Attack/blob/main/AttackNN_Anim.gif)

I use a variant of the Fast Gradient Signed Method to alter images so my own trained ML models misclassify them. I work with the CIFAR-10 Dataset and the MNIST and eplore how hyper paramaters and model classes affect how vulnerable a model is to attack. 

Assuming access to the model, we perform gradient ascent to change our input image as little as possible while making the network misclasify our attacks. We Train 8 Models (see [CIFAR](https://github.com/vs1720/Neural_Attack/blob/main/Train_CIFAR.ipynb) and [MNIST](https://github.com/vs1720/Neural_Attack/blob/main/Train_MNIST.ipynb) training notebooks). 

I found that deeper models are more prone to these attacks, but that their effectiveness can be mitigated using noisy training. While MNIST attacks can be long process, attacks on more complex images - like in the CIFAR dataset - are much quicker. WIth changes so subtle as to be completely imperceptible. 

![image](https://user-images.githubusercontent.com/31740145/131559631-c725ca45-cc14-48c2-bffd-b6f25b384bb2.png)



Check out the [full paper](https://github.com/vs1720/Neural_Attack/blob/main/Attack_NN_paper.pdf)
