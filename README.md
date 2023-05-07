# Unpaired-Image-to-Image-translation

In this project, we aim to solve the problem of image-to-image translation, where usually a mapping is learned between an input image and an output image in a supervised manner. However, in many cases, such paired image data may not be available. We propose a robust solution which will work on non-corresponding pairs of data. Our goal is to learn a mapping  $G : X \to Y$ such that the distribution of images from $G(X)$ is indistinguishable from the distribution Y using an adversarial loss. Because this mapping is highly under-constrained, we couple it with an inverse mapping $F : Y \to X$ and introduce a cycle consistency loss to enforce $F(G(X)) \approx X$ (and vice versa). We then use the method to demonstrate the results on various applications such as style transfer, object transfiguration, etc.

## Repository Structure

- `Implementation/` 
  - Contains `.ipynb` notebooks for end to end training and testing of the model
- `Evaluation/` 
  - Contains`.ipynb` notebooks for model evaluation on different datasets
- `Results/` 
  - Contains train, test results and loss plots for different experiments
- `besthyperparams.json` - Hyperparameters for the best model.

## Authors
- Arushi Arora: aa10350@nyu.edu
- Chandana Thimmalapura Jagadeeshaiah: ct3002@nyu.edu
- Pallabi Chandra: pc3131@nyu.edu
