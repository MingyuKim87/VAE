# Variational Auto Encoding

An implementation of variational auto-encoding (VAE) for MNIST represented by Kingma et al. Paper(2013)
* [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114) by Kingma et al. 
* This implementation is referred from [hwalsuklee’s tutorial](https://github.com/hwalsuklee/tensorflow-mnist-VAE)

Different from the hwalsuklee’s program, this tutorial is not required to use other class file or functional set file.   
Within this IPython notebook, all operations in VAE are performed.


## Results
### Reproduce

Given training set data, VAE architecture can generate the similar images without any label.<br>
In this example, we introduce 2-Dimensional latent space unit. 

* Input Image  
![Input_Image](https://github.com/MingyuKim87/VAE/blob/master/Results/Input_Image.jpg)

* Recounstruction Image  
![Reconstruction_Image](https://github.com/MingyuKim87/VAE/blob/master/Results/PRR.gif)


### Reconstruction

For exploiting latent space in VAE, we generate and put synthetic mesh-grid data (-4:4, -4:4) into the VAE model as hidden variable, Z instead of training set data. 

* Reconstruction Image  
![Reconstruction_Image2](https://github.com/MingyuKim87/VAE/blob/master/Results/PMLR_Reconstruction.gif)

### Learned MNIST manifold

Visualizations of learned data manifold for generative models with 2-dim.<br>
Latent space are given in Figure. 4 in the paper.  


* Manifold Image  
![Manifold_Image](https://github.com/MingyuKim87/VAE/blob/master/Results/PRML_Map.gif)


## References
The implementation is based on the projects:  
[1] https://github.com/oduerr/dl_tutorial/tree/master/tensorflow/vae  
[2] https://github.com/fastforwardlabs/vae-tf/tree/master  
[3] https://github.com/kvfrans/variational-autoencoder  
[4] https://github.com/altosaar/vae  
[5] https://github.com/hwalsuklee/tensorflow-mnist-VAE


## Acknowledgements
This implementation has been performed on Tensorflow 1.7 in Ubuntu 16.04.
