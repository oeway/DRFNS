[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1175282.svg)](https://doi.org/10.5281/zenodo.1175282)

This is a fork of [DRFNS](https://github.com/PeterJackNaylor/DRFNS) for demonstrating how deep learning models can be easily deployed with [ImJoy.io](https://imjoy.io)

This is modified version only support training on synthetic data, for real data, please refer to the [original repository](https://github.com/PeterJackNaylor/DRFNS).

[Run this code with ImJoy](https://imjoy.io/#/app?w=DRFNS&plugin=)



This is the description from the original repository:

```
In this repository, we've implemented the code resulting in the submitted paper "Segmentation of Nuclei in Histopathology Images by deep regression of the distance map." in TMI, by P. Naylor, M. Laé, F. Reyal and T. Walter. The code in this repository is made out of nextflow for pipeline management. For more information about nextflow please refer to [Nextflow's documentation](https://www.nextflow.io/). Each process of this pipeline is made out of python and called via nextflow. Nextflow was very handy to take advantage of a cluster with multi-queues, in particular for a pipeline using CPU's and GPU's.

We tackle the task of nuclei segmentation within histopathology tissue. Many methods have been proposed in the past but relatively few of them try to handle the wide hetereogenity that one can typically encounter with such data. As is the current trend, we apply state of the art algorithm technics based on CNN but also our novel nuclei segmentation framework. We compare each method with two metrics, the first pixel based and the second objected based. We elaborate a benchmark of fully convolutionnal algorithm applied to these datasets.  In particular we compare ourselves to [\[Neeraj et al\]](https://nucleisegmentationbenchmark.weebly.com/) and show that our deep regression method outperforms previous state of the art method for separating cluttered objects.
```
