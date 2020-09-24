# Aravindan

In these models, a generator network attempts to map samples from a simple low-dimensional distribution (such as standard
Gaussian) to points in a high-dimensional space that resemble the learned data distribution. At the
same time, a discriminator network attempts to distinguish between real and generated samples.
By setting up a min-max game between them, the two networks are jointly trained. The latent
probability distribution along with the learned generator network define a stochastic procedure that
can produce new samples. The adversarial framework has been shown to be extremely successful
in modeling complex distributions [Berthelot et al. (2017); Vondrick et al. (2016); Pascual et al.
(2017); Wu et al. (2016)], and the priors induced by these models are useful for various applications
[Shrivastava et al. (2016); Ho & Ermon (2016)]

r = real distribution
g = generated distribution
y = observed noisy image
x = clean signal
n = noise

[AMBIENT-GANS](https://www.cs.utexas.edu/~ecprice/papers/ambientgan.pdf)
---
* Learns the underlying distribution from only noisy images.
* They use a noise simulation model assuming prior information about the noise is known and incorporate this the adversial training framework.


our discriminator must distinguish a real
measurement from a simulated measurement of a generated image;

Our method is able to construct good generative models from extremely noisy observations and
even from low dimensional projections with drastic per-sample information loss

We consider the task of learning an implicit generative model given only lossy measurements of samples from the distribution of interest. We show that the true underlying distribution can be provably recovered even in the presence of per-sample
information loss for a class of measurement models

We first consider measurements that are noisy, blurred versions of the desired
images. That is, we consider convolving the original image with a Gaussian kernel and adding
independent Gaussian noise to each pixel (our actual theorem applies to more general kernels and
noise distributions). Because of the noise, this process is not invertible for a single image. However,
we show that the distribution of measured images uniquely determines the distribution of original
images. This implies that a pure Nash equilibrium for the GAN game must find a generative model
that matches the true distribution. 

The idea of operating generators and discriminators on different spaces has been proposed before.
[Neyshabur et al. (2017)] explores an interesting connection of training stability with low dimensional projections of samples. They show that training a generator against an array of discriminators,
each operating on a different low-dimensional projection of the data can improve stability.

Write equations **4(1)**
**GET THE ARCHITECTURE**

---


