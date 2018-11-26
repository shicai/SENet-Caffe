# SENet-Caffe

### Introduction

This is a Caffe implementation of Squeeze-and-Excitation Networks (SENet). For details, please read the original slides:
- [Squeeze-and-Excitation Networks](http://image-net.org/challenges/talks_2017/SENet.pdf)

For offical implementations, please check this repo [SENet](https://github.com/hujie-frank/SENet).

### Pretrained Models on ImageNet

Here we provide a pretrained SE-ResNet-50 model on ImageNet, which achieves slightly better accuracy rates than the original one reported in the official repo. You can use the official [bvlc caffe](https://github.com/BVLC/caffe) to run this model without any modifications.

The top-1/5 accuracy rates by using single center crop (crop size: 224x224, image size: 256xN):

Network|Top-1|Top-5|Download|Architecture
:---:|:---:|:---:|:---:|:---:
SE-ResNet-50| 78.01| 94.21| [caffemodel (107 MB)](https://drive.google.com/open?id=0B7ubpZO7HnlCWkwtSG5CdXBKcmc)| [netscope](http://ethereon.github.io/netscope/#/gist/36a20d27cba38695b4a44632d7af608c), [netron](http://lutzroeder.github.io/netron?gist=36a20d27cba38695b4a44632d7af608c)

For your convenience, we also provide a link to this model on [Baidu Disk](https://pan.baidu.com/s/1eSzT6KU).


### Notes

- BGR mean values **[103.94,116.78,123.68]** are subtracted
- **scale: 0.017** is used as std values for image preprocessing
- Images labels are the same as [fb.resnet.torch](https://github.com/facebook/fb.resnet.torch). We also provide `synset.txt`, which can be found [here](https://gist.github.com/shicai/fa9f98edc23521382955d4731636d1af).
