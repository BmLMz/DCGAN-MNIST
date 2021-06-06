# DCGAN-MNIST
* This small personnal project is inspired from DCGAN Pytorch Tutorial. 
The purpose is to test stability of DCGAN on a toy-set such as MNIST. I tried several architecures for discriminator and the generator and different optimizers.
DCGAN is a really powerfull tool, but it seems really hard to get convergence on a simple problem such as MNIST. I have observe *Mode collapse* many time when
building my networks, which is ubquitous in DCGAN, these models suffer a lot from it.
* One of the main solutions I looked at is the implementation of a <a href = 'https://github.com/martinarjovsky/WassersteinGAN'>**Wasserstein GAN**</a>.
* Besides the simple architectures developped in the notebook, I finaly used the following parameters:
  - lr-gen = 0.0002
  - lr-dis = 0.0002
  - optimizer-gen = Adam
  - optimizer-dis = SGD
  - 100 epochs
