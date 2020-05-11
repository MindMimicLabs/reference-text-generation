# Sample - Text Generation

Text generation can be thought of as a prediction problem.
Given N tokens, what is the next token.
As text is a categorical variable, this in turn can be thought of as a classification problem.

The goal of this repository is to demonstrate simple techniques in both R and Python for performing text generation using deep learning. 

## Scripts

The scripts below are available for both R and Python.
The names of the files will be identical except for the extension, either `.r` or `.py`.
The code is broken up into different files to help highlight the language differences while maintaining the structural elements of the process.
Any configuration differences have been extracted into a `.yml` file of the same name.

* `~/code/dnn_model.{r|py}` defines the deep learning model.
  In this case it is a single `LSTM` followed by a `Dense`.
  In a _real_ setting the network would have more layers.
  Unfortunately, hyper-tuning a multi-layer network is as much _art_ as science.
  To keep this example on-point, the simplest version was chosen.

## Environment

Tensor Flow is super fickle when it comes to setup.
The code used in this paper uses the v1 guidance found [here](https://github.com/MindMimicLabs/getting-started/blob/master/setup-your-environment.md)
