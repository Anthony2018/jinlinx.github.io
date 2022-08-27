---
layout: page
title: Neural Style Transfer Project
description: CSE Deep Learning Neural Style Transfer Project, Seattle, WA, 09/2019 – 12/2019
img:
importance: 1
category: Project
---

**[code available](https://github.com/Anthony2018/CSE599-Project-NST)**

# **Introduction:**

Human artists usually master special skills to paint a picture with a unique style, which makes them look different even for same object, like oil painting, abstract painting and impressionist painting. There are some software filters that changes the appearance of an image or part of an image by altering the shades and colors of the pixels as well as adding tones and special effects to a picture. However, the effect of those filters is usually limited and could only transfer the image to a predefined simple style. Our goal and motivation are implementing an algorithm that has the ability to transfer the style of one picture according to a new given picture, which just like some artists could do. We know that convolution neural networks can transfer an image into feature map. Hence the idea of our project is trying to produce a new image who has similar features to those two input images. In this way, we could create a high perceptual quality artistic image that keeps the content of one image and the style of the other. In normal style transfer, the color of the output will affect the output. Hence, we also implement a method that could keep the color of content image. And cool thing in this project is that we can do the faster transfer and unchanged color feature.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/NST/poster.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Poster
</div>

# **Related work:** 

Base on the paper written by Gatys and Johnson, we implement the neural style transfer, neural style transfer with color preserving, fast neural style transfer and fast neural style transfer with color preserved by ourselves. There are some existing implementations of first three work, the one we contribute to the problem is fast neural style transfer with color preserving, the key idea is to run color preserved to compute a unique style image for each image in whole training data.The training data for fast neural style transfer with and with color transfer is coco-2014 train image.

# **Conclusion**

1.The style transfer algorithm performs an obvious changing on visual perspective. It demonstrates that the feature map got from the structure of CNN did represent the visual style of an image to a certain extent.

2.The color keeps unchanged to some degree after using the color preserved algorithm.

3.The FNST takes less time to compute the result, which is enough for an GXT1060 to generate a smooth transferred video.

# **Future work** 

1. We could try to generate a segmentation result, which only make a specific part of the output to be transferred. 

2. From the perspective of software, we could develop an application that could get the picture from user, and thus improve the experience of users.

# Reference

Gatys, Leon A., Alexander S. Ecker, and Matthias Bethge. "Image style transfer using convolutional neural networks." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

Gatys, L. A., Bethge, M., Hertzmann, A., & Shechtman, E. (2016). Preserving color in neural artistic style transfer. arXiv preprint arXiv:1606.05897.

Johnson, J., Alahi, A., & Fei-Fei, L. (2016, October). Perceptual losses for real-time style transfer and super-resolution. In *European conference on computer vision* (pp. 694-711). Springer, Cham.