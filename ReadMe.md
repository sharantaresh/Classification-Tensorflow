Fine grained classification of images comes with number of challenges. To overcome this, the method suggested here is using inception block as headf to VGG16 base model.


Base Model Selected for the Assignment: **VGG16**

<img width="487" alt="image" src="https://user-images.githubusercontent.com/119483443/204999716-1d98550a-d0f1-447d-9aa6-33e1c49a17c3.png">


Models Modifications
VGG16 with **Inception Block** and **Scaled exponential linear activation**

**Inception Block**

It allows the internal layers to pick and choose which filter size will be relevant to learn the required information. So even if the size of the target in the image is different, the layer works accordingly to recognize the target. In the present Model, this benefit of Inception block originally used in Inception v1 is used to extract feature from the images depending upon the size of the pack or text written on the pack.

<img width="446" alt="image" src="https://user-images.githubusercontent.com/119483443/204999209-6887609a-a3cc-44a5-bcf1-0d14aa49f2a1.png">


**Scaled Exponential linear unit**

It deals with two major parts of Model Training:
1.	It does internal normalization which means network converges faster compared to external normalization.
2.	Vanishing and exploding gradient problem is not possible.
