## Overview

In this project, I explore various deep learning frameworks and model architectures to predict satellite images of typhoons. After thorough experimentation with TensorFlow and different model architectures, I ultimately chose to implement a Convolutional Neural Network (CNN) combined with a Long Short-Term Memory (LSTM) network using PyTorch.

## Implementation Details

The entire process, from data exploration to model training, is documented in the 'image_generation_usage.ipynb' file. Below are some of the key steps involved:

1. **Data Preprocessing:**
   - Sliding Window Approach: I utilised a sliding window technique to load time-series data, ensuring the model captures sequential patterns effectively. The final model uses a sliding window of size 5.
2. **Environment Compatibility:**
   - Colab Compatibility: The image_generation_usage.ipynb' file is designed to run seamlessly on Google Colab, allowing for easy collaboration and access to GPU resources.
   - Local Environment: The project can also be executed in an environment with the required dependencies listed in 'requirements.txt' (torch, etc.).
3. **Prediction of future trajectories:**
   - The 'CNNLSTM_final' class within the notebook is responsible for defining CNN-LSTM architecture model.
   - Generating Future Images: The notebook includes an example where the model predicts and generates three successive satellite images based on the input of a surprise storm image.

Future Work

- Try out other models (GANs, Diffusion Models, Transformers etc)

- Try transfer learning

- Try to find mutli-channel input data rather than using more than just Image data (I.e. a model that takes as input image data and previous wind speed) 

  

**Note that this is my contribution to a university project. For my contribution I received a Distinction.**