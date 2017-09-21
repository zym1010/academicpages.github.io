---
title: "Software"
permalink: /software/
author_profile: true
---

During my Ph.D. career, I have developed many open-source software projects for the lab. Many of these projects are hosted under the [lab's GitHub account](https://github.com/leelabcnbc/), and I wrote over 99% of the code.

# Computer vision, computational neuroscience


## computer vision

* [leelab-toolbox](https://github.com/leelabcnbc/leelab-toolbox) This is supposed to be the package shared by all the lab people. It contains many utility functions for image preprocessing, CNN feature extraction, and stereo vision.
* [cnnvis-pytorch](https://github.com/leelabcnbc/cnnvis-pytorch) Visualization of CNN in PyTorch.
* [pytorch-caffe-models](https://github.com/leelabcnbc/pytorch-caffe-models) Standard Caffe models in PyTorch.

## neural data modeling

* [strflab-python](https://github.com/leelabcnbc/strflab-python/) A Python library with functionality similar to [STRFlab](http://strflab.berkeley.edu/). It contains spike-triggered methods, GLM models, etc.
* [early-vision-toolbox](https://github.com/leelabcnbc/early-vision-toolbox/) A collection of models and analysis methods for early visual areas. Most of its functionalities have been incorporated into `leelab-toolbox`.

## neural data preprocessing

* [cdttable-matlab](https://github.com/leelabcnbc/cdttable-matlab) A MATLAB program designed to convert trial-based spiking neural data into a universal format (CDT table) for later analysis.
* [cdttable-python](https://github.com/leelabcnbc/cdttable-python) a Python rewrite of `cdttable-matlab`, allowing much more flexible data formats.

 
# Data management

* [DataSMART](https://github.com/leelabcnbc/datasmart) DataSMART is for Scalable Management and Analytic Research Tools for Data. It's used in the lab to manage data and processing pipelines.
 
# DevOps

* [DevOps](https://github.com/leelabcnbc/DevOps) a bunch of DevOps files for using scientific Python environments in a cluster system, without root privileges. In particular, it helps installing newer Deep Learning tools (torch, TensorFlow) that normally require newer compiler and system libraries easier to install on older operating systems, such as CentOS 6. This project is used by most of the GPU users on [CNBC cluster](http://www.cnbc.cmu.edu/resources/computing-resources/).

# Miscellaneous.

* [lab-wiki-builder](https://github.com/leelabcnbc/lab-wiki-builder) a tool for building wiki website for academic labs.

In addition, I have made minor contributions to the following open source projects.

* [conda-forge](https://conda-forge.org/)
* [pandas](http://pandas.pydata.org/)
* [scikit-learn](http://scikit-learn.org/)
* [TensorFlow models](https://github.com/tensorflow/models)
