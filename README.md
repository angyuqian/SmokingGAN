# SmokingGAN
An experimental framework for running ML Models inside the Grasshopper / Rhino environement

## Attributions
SmokingGAN is a Hackathon project for the 2020 AEC Tech Symposium organized by CORE Studio at Thornton Tomasetti

This project has been a collaborative effort between [Mayur Mistry](https://github.com/Mistrymm7), [Sergey Pigach](https://github.com/enmerk4r), [Charlie Portelli](https://github.com/Crashnorun) and [Sergio Guindon](https://github.com/sguindon)

**SmokingGAN borrows heavily from the following open-source projects:**

**Fast Style Transfer**: https://github.com/lengstrom/fast-style-transfer

**TF Monodepth 2**: https://github.com/FangGet/tf-monodepth2

## Description
SmokingGAN is an attempt at incorporating GANs into a Rhino / Grasshopper design workflow. The two major parts of the SmokingGAN are the Flask server exposing pre-trained checkpoints (This hackathon version currently serves [A Style GAN](https://github.com/lengstrom/fast-style-transfer) and a [Depth Map generator](https://github.com/FangGet/tf-monodepth2), but can be extended to work with any other pretrained checkpoints) and a Grasshopper plugin that accesses the Flask API and also provides functionality for converting images to meshes based on the depth information.

![Flythrough](https://github.com/enmerk4r/SmokingGAN/blob/main/Assets/FlyThrough.gif)

This is the basic architectural diagram showing the main components of the API:

![Diagram](https://github.com/enmerk4r/SmokingGAN/blob/main/Images/Image%20GAN%20Flow%20Chart.png)
 
 ## Setup
 We recommend creating an Anaconda environment with **Python 3.7** (IMPORTANT: we've ran into serious issues with Tensorflow and Python 3.8)
 ```
 conda create --name your-env-name python=3.7
 ```
 
 **Pretrained Checkpoint Files** 
 
 
 ***Style Transfer*** - https://drive.google.com/drive/folders/0B9jhaT37ydSyRk9UX0wwX3BpMzQ
 
 
 ***Depth Map*** - https://drive.google.com/drive/folders/0B9jhaT37ydSyRk9UX0wwX3BpMzQ
