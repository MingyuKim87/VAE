# VAE

An implementation of variational auto-encoder (VAE) for MNIST represented by Kingma et al. Paper(2013)
* [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114) by Kingma et al. 
* This implementation is referred from [hwalsuklee’s tutorial](https://github.com/hwalsuklee/tensorflow-mnist-VAE)

Different from the hwalsuklee’s program, this tutorial is not required to use other class file or functional set file. Within IPython notebook file, all operations in VAE are performed.


## Result
### Reproduce

Given training set data, VAE architecture can generate the similar images without any label. 
In this example, we introduce 2-Dimensional latent space unit. 

<table align = ‘center’>
<tr align = ‘center’>
<td> Input Image </td>
<td> Reproduced Image </td>
</tr>
<tr>
<td><img src = ‘Results/Input_Image.jpg’ height = ‘150px’>
<td><img src = ‘Results/Reconstruction_1.gif’ height = ‘150px’>
</tr>
</table>

### Reconstruction

For exploiting latent space in VAE, we generate and put synthetic mesh-grid data (-4:4, -4:4) into the VAE model as hidden variable, Z instead of training set data. 


<table align = ‘center’>
<tr align = ‘center’>
<td> Reproduced Image from synthetic latent space </td>
</tr>
<tr>
<td><img src = ‘Results/Reconstruction_2.gif’ height = ‘150px’>
</tr>
</table>

### Learned MNIST manifold

Visualizations of learned data manifold for generative models with 2-dim. latent space are given in Figure. 4 in the paper.  


<table align = ‘center’>
<tr align = ‘center’>
<td> Distribution of labeled data </td>
</tr>
<tr>
<td><img src = ‘Results/Manifold_learning.gif’ height = ‘150px’>
</tr>
</table>

## References
The implementation is based on the projects:  
[1] https://github.com/oduerr/dl_tutorial/tree/master/tensorflow/vae  
[2] https://github.com/fastforwardlabs/vae-tf/tree/master  
[3] https://github.com/kvfrans/variational-autoencoder  
[4] https://github.com/altosaar/vae
[5] https://github.com/hwalsuklee/tensorflow-mnist-VAE

## Acknowledgements
This implementation has been performed in Tensorflow 1.7 on Ubuntu 16.04.