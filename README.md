# CycleGAN
### [PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix) | [project page](https://junyanz.github.io/CycleGAN/) |   [paper](https://arxiv.org/pdf/1703.10593.pdf)

Torch implementation for learning an image-to-image translation (i.e. [pix2pix](https://github.com/phillipi/pix2pix)) **without** input-output pairs, for example:



<img src="https://junyanz.github.io/CycleGAN/images/teaser_high_res.jpg" width="1000px"/>

[Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://junyanz.github.io/CycleGAN/)  
 [Jun-Yan Zhu](https://people.eecs.berkeley.edu/~junyanz/)\*,  [Taesung Park](https://taesung.me/)\*, [Phillip Isola](http://web.mit.edu/phillipi/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/)  
 Berkeley AI Research Lab, UC Berkeley  
 In ICCV 2017. (* equal contributions)  

This package includes CycleGAN, [pix2pix](https://github.com/phillipi/pix2pix), as well as other methods like [BiGAN](https://arxiv.org/abs/1605.09782)/[ALI](https://ishmaelbelghazi.github.io/ALI/) and Apple's paper [S+U learning](https://arxiv.org/pdf/1612.07828.pdf).  
The code was written by [Jun-Yan Zhu](https://github.com/junyanz) and [Taesung Park](https://github.com/taesung).  
**Update**: Please check out [PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix) implementation for CycleGAN and pix2pix.
The PyTorch version is under active development and can produce results comparable or better than this Torch version.

## Other implementations:
<p><a href="https://github.com/leehomyc/cyclegan-1"> [Tensorflow]</a> (by Harry Yang),
<a href="https://github.com/architrathore/CycleGAN/">[Tensorflow]</a> (by Archit Rathore),
<a href="https://github.com/vanhuyz/CycleGAN-TensorFlow">[Tensorflow]</a> (by Van Huy),
<a href="https://github.com/XHUJOY/CycleGAN-tensorflow">[Tensorflow]</a> (by Xiaowei Hu), 
<a href="https://github.com/LynnHo/CycleGAN-Tensorflow-Simple"> [Tensorflow-simple]</a> (by Zhenliang He),
<a href="https://github.com/luoxier/CycleGAN_Tensorlayer"> [TensorLayer]</a> (by luoxier),
<a href="https://github.com/Aixile/chainer-cyclegan">[Chainer]</a> (by Yanghua Jin),
<a href="https://github.com/yunjey/mnist-svhn-transfer">[Minimal PyTorch]</a> (by yunjey),
<a href="https://github.com/Ldpe2G/DeepLearningForFun/tree/master/Mxnet-Scala/CycleGAN">[Mxnet]</a> (by Ldpe2G),
<a href="https://github.com/tjwei/GANotebooks">[lasagne/Keras]</a> (by tjwei), 
<a href="https://github.com/simontomaskarlsson/CycleGAN-Keras">[Keras]</a> (by Simon Karlsson)</p>
</ul>

## Applications
### Monet Paintings to Photos
<img src="https://junyanz.github.io/CycleGAN/images/painting2photo.jpg" width="1000px"/>

### Collection Style Transfer
<img src="https://junyanz.github.io/CycleGAN/images/photo2painting.jpg" width="1000px"/>

### Object Transfiguration
<img src="https://junyanz.github.io/CycleGAN/images/objects.jpg" width="1000px"/>

### Season Transfer
<img src="https://junyanz.github.io/CycleGAN/images/season.jpg" width="1000px"/>

### Photo Enhancement: Narrow depth of field
<img src="https://junyanz.github.io/CycleGAN/images/photo_enhancement.jpg" width="1000px"/>



## Prerequisites
- Linux or OSX
- NVIDIA GPU + CUDA CuDNN (CPU mode and CUDA without CuDNN may work with minimal modification, but untested)
- For MAC users, you need the Linux/GNU commands `gfind` and `gwc`, which can be installed with `brew install findutils coreutils`.

## Getting Started
### Installation
- Install torch and dependencies from https://github.com/torch/distro
- Install torch packages `nngraph`, `class`, `display`
```bash
luarocks install nngraph
luarocks install class
luarocks install https://raw.githubusercontent.com/szym/display/master/display-scm-0.rockspec
```
- Clone this repo:
```bash
git clone https://github.com/junyanz/CycleGAN
cd CycleGAN
```
