[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1175282.svg)](https://doi.org/10.5281/zenodo.1175282)

This is a fork of [DRFNS](https://github.com/PeterJackNaylor/DRFNS) to demonstrate how deep learning models can be easily deployed with [ImJoy.io](https://imjoy.io).

This modified version only support training on synthetic data, for real data, please refer to the [original repository](https://github.com/PeterJackNaylor/DRFNS).

# Run DRFNS-Lite with ImJoy.io

## Setup
Choose a version and click install:

[DRFNS-Lite (CPU Version)](https://imjoy.io/#/app?w=DRFNS&plugin=https://raw.githubusercontent.com/oeway/DRFNS-Lite/master/DRFNS-Lite.imjoy.html&tag=CPU)

[DRFNS-Lite (GPU Version)](https://imjoy.io/#/app?w=DRFNS&plugin=https://raw.githubusercontent.com/oeway/DRFNS-Lite/master/DRFNS-Lite.imjoy.html&tag=GPU)

Once installed Click `DRFNS-Lite` in the plugin menu and follow the instructions in the dialog to install the Python Plugin Engine.


## Usage

In the [ImJoy web app](https://imjoy.io/#/app?w=DRFNS), expand the DRFNS-Lite plugin menu and click step by step or add then into the workflow.

<img src="https://raw.githubusercontent.com/oeway/DRFNS-Lite/master/img/plugin-menu-screenshot.png" width="200"> <img src="https://raw.githubusercontent.com/oeway/DRFNS-Lite/master/img/workflow-screenshot.png" width="200">

## Run the Python engine remotely
The actual calculations are performed by the ImJoy plugin engine. By default, this engine runs on the local machine. However, some of the calculations during the training are time-consuming. For faster processing, they are ideally performed on GPUs. ImJoy allows to launch the plugin engine on a remote machine, e.g. a GPU server. For more instrucation please consult the [ImJoy User Manual](https://imjoy.io/docs/index.html#/user-manual?id=use-the-python-engine-remotely).

## About DRFNS

This is the description from the original repository:

In this repository, we've implemented the code resulting in the submitted paper "Segmentation of Nuclei in Histopathology Images by deep regression of the distance map." in TMI, by P. Naylor, M. Laé, F. Reyal and T. Walter.

We tackle the task of nuclei segmentation within histopathology tissue. Many methods have been proposed in the past but relatively few of them try to handle the wide hetereogenity that one can typically encounter with such data. As is the current trend, we apply state of the art algorithm technics based on CNN but also our novel nuclei segmentation framework. We compare each method with two metrics, the first pixel based and the second objected based. We elaborate a benchmark of fully convolutionnal algorithm applied to these datasets.  In particular we compare ourselves to [\[Neeraj et al\]](https://nucleisegmentationbenchmark.weebly.com/) and show that our deep regression method outperforms previous state of the art method for separating cluttered objects.
