# High-Resolution-Image-using-SRGAN

INTRODUCTION

The demand for high-resolution images is pervasive across various domains, including medical imaging, satellite imagery, surveillance, and digital photography. However, acquiring high-resolution images may not always be feasible due to hardware limitations or practical constraints. To address this challenge, Super-Resolution Generative Adversarial Network (SRGAN) offers a promising solution by employing deep learning techniques to generate high-resolution images from low-resolution inputs.


MODEL ARCHITECTURE

The model is assembled from two components Discriminator and Generator.  
Discriminator - Responsible to distinguish between generated photos and real photos. 
Generator - Generate high resolution images from low resolution images.

![image](https://github.com/DaffneyChristina/High-Resolution-Image-using-SRGAN/assets/107945264/eb3fe0ba-e7ee-49a7-8198-5efd4ff53aac)

Generator
7 Convolution blocks Each block with the same number of filters
PReLU with ( α = 0.2 ) is used as activation layer
2 PixelShuffler layers for upsampling - PixelShuffler is feature map upscaling
Skip connections are used to achieve faster convergence

Discriminator
16 Residual blocks Each block with increasing number of filters
LeakyReLU with ( α = 0.2 ) is used as activation layer
2 Dense layers

![image](https://github.com/DaffneyChristina/High-Resolution-Image-using-SRGAN/assets/107945264/909ed512-8b3c-4c90-a1b1-fb1d1039d9b5)

DATASET
202,599 number of face images of various celebrities
10,177 unique identities, but names of identities are not given
40 binary attribute annotations per image
5 landmark locations

OUTPUT

![image](https://github.com/DaffneyChristina/High-Resolution-Image-using-SRGAN/assets/107945264/af66a0ee-0d7c-4a9c-a2ff-ed790974f6cc)










