# Variational Autoencoders (VAE) & Conditional Variational Autoencoders (CVAE) 🚀

This repository contains the implementation of Variational Autoencoders (VAE) and Conditional Variational Autoencoders (CVAE). These models are a type of generative model used to learn complex distributions and generate new data samples.

# What is VAE? 🤖
A Variational Autoencoder (VAE) is a type of generative model that uses a probabilistic approach to learn the underlying structure of the data. It consists of an encoder and a decoder. The encoder maps the input data to a latent space distribution, and the decoder reconstructs the data from this distribution.

The main idea is to approximate the true posterior distribution of the data in the latent space.


Key Variables:

• x: The input data (e.g., images, text).

• z: The latent variables (i.e., compressed representation of the data).

• μ: Mean of the latent distribution.

• σ: Standard deviation of the latent distribution.

• p(z): Prior distribution of the latent variables (usually a Gaussian distribution).

# VAE Equation 🔢
The VAE optimization objective can be written as: 
![image1](https://github.com/user-attachments/assets/2f39d660-f413-47fb-8178-db7fc4a56c03)


# What is CVAE? 🧠
A Conditional Variational Autoencoder (CVAE) is an extension of the VAE that conditions the latent variables on additional information, such as labels or other attributes. This allows the model to generate data conditioned on certain factors, such as generating images of a particular class or generating text in a particular style.

In CVAE, we condition both the encoder and the decoder on an additional variable y (such as a class label).

Key Variables:

• x: The input data (e.g., images, text).

• y: The conditional variable (e.g., class labels).

• z: The latent variables.

• μ: Mean of the latent distribution conditioned on 


• σ: Standard deviation of the latent distribution conditioned on 

# CVAE Equation 📏

The CVAE optimization objective can be written as:

![image2](https://github.com/user-attachments/assets/aef4e894-c3c3-43ea-a6bd-8b47033bad1c)


To provide an example, let's suppose we've trained an autoencoder model on a large dataset of faces with a encoding dimension of 6. An ideal autoencoder will learn descriptive attributes of faces such as skin color, whether or not the person is wearing glasses, etc. in an attempt to describe an observation in some compressed representation.

![mage3](https://github.com/user-attachments/assets/c0f34f44-b903-49be-9a58-a18a82a0a077)



# Additional Resources (For Further Clarification) 🖥
[![Variational Autoencoders](https://img.youtube.com/vi/9zKuYvjFFS8/0.jpg)](https://www.youtube.com/watch?v=9zKuYvjFFS8)

> 📚 This video is a great resource for further clarification on Variational Autoencoders. You can check it out here: [Variational Autoencoders - YouTube](https://www.youtube.com/watch?v=9zKuYvjFFS8)

# Reference 
> 📚 For further information, please refer to the article on Variational Autoencoders by Jeremy Jordan: [Jeremy Jordan's Variational Autoencoders Article](https://www.jeremyjordan.me/variational-autoencoders/)

