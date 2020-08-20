# DLclass-Oliver_Inpainting
Code and Demo of the homework paper for DL class in UPC. 

"A Context-Based Multi-Scale Discriminant Model for Natural Image Inpainting".

## Note
It is a model for inpainting task, which is based on [Global & Local](https://dl.acm.org/doi/abs/10.1145/3072959.3073659),

## Demo(Inference)
### 1. Download pretrained generator

* [Required] Pretrained generator model (Completion Network): [Baidu NetDisk](https://pan.baidu.com/s/1J8rrUW8K0Cw2L94sgMI-vQ) (key: 1234)
* [Optional] Pretrained discriminator model (Context Discriminator): [Baidu NetDisk](https://pan.baidu.com/s/1r2T4AKA0S96q0HqV62SC3g) (key: 5678)

Note that you don't need the dicriminator model for inference because only generator is necessary to perform image completion.

Both the generator and discriminator were trained on the CelebA. 

### 2. Inference

```
# in {path_to_this_repo}/,
$ python predict.py model_cn config.json images/test.jpg output.jpg
```

## Demo(Training)
One can also train the network with their own datasets, by modifying the data path in `config.json`.

### 1. Prepare the dataset
Here we offer some official links used in paper.
* [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)
* [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)
* [Imagenet](http://www.image-net.org/)
* [LSUN](https://www.yf.io/p/lsun)
* [ParisStreetView](https://github.com/pathak22/context-encoder#6-paris-street-view-dataset) (Request permission through e-mail)

Process the data by running `/datasets/make_dataset.py` .
### 2. Training

## Results
### 1. Reuslts on ParisStreet View dataset along with epochs.
![All text](https://github.com/Oliiveralien/DLclass-Oliver_Inpainting/blob/master/images/GIF%202020-8-20%2010-56-41.gif)
