# DLclass-Oliver_Inpainting
Code and Demo of the homework paper for DL class in UPC. 

"A Context-Based Multi-Scale Discriminant Model for Natural Image Inpainting".

## Introductoin
Image inpainting is a classical yet challenging problem in computer vison with many real-world applications. In this paper, we propose a novel method for inpainting based on Convolutional Neural Network (CNN) and Generative Adversarial Networks (GAN). By analogy with the autoencoder, a new context encoder is proposed to generate the contents of a missing image region conditioned on its surroundings. To improve the stability and efficiency, we also modify the architecture of the context encoder by introducing 1*1 convolution, as well as other improvements. In addition, a multi-scale discriminator combining with GAN is presented. During training, the reconstruction and adversarial losses are used for the global image. To generate more details, we further add a local texture loss for the missing part. Qualitative experiments show that our model performs favorably against classical methods in generating visually plausible inpainting results. Moreover, quantitative experiments substantiate the effectiveness of the proposed method in natural image inpainting.

## Note
It is a model for inpainting task, which is based on [Global & Local](https://dl.acm.org/doi/abs/10.1145/3072959.3073659).

## Results
![All text](https://github.com/Oliiveralien/DLclass-Oliver_Inpainting/blob/master/images/GIF%202020-8-20%2010-56-41.gif)
