# FLUX.1-dev Image Generation

This project contains a Python script for generating images from text prompts using the FLUX.1-dev text-to-image model. The script is adapted from a Jupyter Notebook and is designed to run in an environment like Google Colab.

## Description

The script performs the following steps:
1.  Installs necessary Python packages, including `torch`, `diffusers`, and `accelerate`.
2.  Clones the `Multi-image-gen-colab` repository to leverage its helper scripts and model management.
3.  Downloads pre-trained model weights for the FLUX.1 UNET, the VAE, and text encoders (CLIP-L and T5-XXL).
4.  Loads the models into memory.
5.  Iterates through a predefined list of text prompts.
6.  For each prompt, it generates an image using a guided diffusion process.
7.  Saves the generated images as PNG files.
