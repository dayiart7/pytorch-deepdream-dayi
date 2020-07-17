## Deep Dream :computer: + :ocean::zzz: = :heart:
This repo contains PyTorch implementation of the Deep Dream algorithm (:link: blog by [Mordvintstev et al.](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)).

<p align="center">
<img src="data/examples/figures_width_600_model_VGG16_IMAGENET_relu4_3_pyrsize_12_pyrratio_1.4_iter_10_lr_0.09_shift_32.jpg" width="600"/>
</p>

### What is Deep Dream algorithm?
In a nutshell the algorithm maximizes activations of chosen network layers (1 or multiple) by doing gradient descent.

So from an input image like the one of the left after "dreaming" we get the image on the right:
<p align="center">
<img src="data/input/figures.jpg" width="400"/>
<img src="data/examples/figures_width_600_model_VGG16_IMAGENET_relu4_3_pyrsize_4_pyrratio_1.4_iter_10_lr_0.09_shift_41.jpg" width="400"/>
</p>

Who would have said that neural networks had this creativity hidden inside. :heart:

### Why yet another Deep Dream repo?

Most of the original Deep Dream repos were written in **Caffe** and the ones written in PyTorch are usually of low quality or really hard to read.

This repo is an attempt of making the **cleanest** DeepDream repo that I'm aware of + it's written in **PyTorch!** :heart:

All of the examples have parameters used to create them encoded into the file name, so you can either reconstruct them
or create new ones - although there is some randomness in the process so identical reconstructions are not guaranteed.

## Examples

*Note: all of the deepdream images were produced by me (using this repo), credits for original image artists [are given bellow](#acknowledgements).*

## Setup

1. Open Anaconda Prompt and navigate into project directory `cd path_to_repo`
2. Run `conda env create` (while in project directory)
3. Run `activate pytorch-deepdream`

That's it! It should work out-of-the-box executing environment.yml file which deals with dependencies.

-----

PyTorch package will pull some version of CUDA with it, but it is highly recommended that you install system-wide CUDA beforehand, mostly because of GPU drivers. I also recommend using Miniconda installer as a way to get conda on your system. 

Follow through points 1 and 2 of [this setup](https://github.com/Petlja/PSIML/blob/master/docs/MachineSetup.md) and use the most up-to-date versions of Miniconda and CUDA/cuDNN.
(I recommend CUDA 10.1 as it is compatible with PyTorch 1.5, which is used in this repo, and newest compatible cuDNN)

## Usage


### Debugging/Experimenting


## Acknowledgements

I found these repos useful: (while developing this one)
* [deepdream](https://github.com/google/deepdream) (Caffe, original repo)
* [DeepDreamAnim](https://github.com/samim23/DeepDreamAnim) (Caffe)
* [AI-Art](https://github.com/Adi-iitd/AI-Art/blob/master/DeepDream.py) (PyTorch)
* [neural-dream](https://github.com/ProGamerGov/neural-dream) (PyTorch)
* [DeepDream](https://github.com/CharlesPikachu/DeepDream) (PyTorch)

I found the images I was using here:
* [awesome figures pic](https://www.pexels.com/photo/action-android-device-electronics-595804/)
* [awesome bridge pic](https://www.pexels.com/photo/gray-bridge-and-trees-814499/)

Other images are now already classics in the NST and DeepDream worlds.

## Citation

If you find this code useful for your research, please cite the following:

```
@misc{Gordić2020DeepDream,
  author = {Gordić, Aleksa},
  title = {pytorch-deepdream},
  year = {2020},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/gordicaleksa/pytorch-deepdream}},
}
```

## Licence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/gordicaleksa/pytorch-deepdream/blob/master/LICENCE)