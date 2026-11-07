---
layout: default
---

**Name:** Taejun Park  
**UCSD email:** tap008@ucsd.edu  
**Section:** D13 — Analysis of high-dimensional neural data  
**Mentor:** Professor Mikio Aoi

**1. What is the most interesting topic covered in your domain this quarter?**  
I found representational similarity analysis (RSA) most interesting. In our Allen Institute exercises, we could compare how two visual areas organized the same set of trials even though the regions contained different neurons. That made me wonder whether a low-dimensional embedding could preserve enough information to decode a stimulus while changing which trials look similar to one another.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**  
I would investigate how much information about the direction of a moving visual stimulus survives dimensionality reduction in mouse visual cortex. Using Allen Brain Observatory recordings, I would start with primary visual cortex (VISp) and a higher visual area (VISal). I would compare PCA and an autoencoder at matched dimensions, using decoding accuracy on held-out trials to measure how much stimulus information remains and RSA to measure how much the geometry of the original trial responses changes.

**3. What is a potential change you’d make to the approach taken in your current Quarter 1 Project?**  
For the rotated MNIST project, I would train separate decoders for digit identity and rotation angle at each layer. I would evaluate both on the same held-out source images and keep all rotated versions of a given image in the same split. That would let me test whether later layers retain enough information to recognize the digit while losing information about how it was rotated.

**4. What other techniques would you be interested in using in your project?**  
I would use nearest-neighbor overlap to check whether individual trials keep the same neighbors after compression. I would also try a Poisson autoencoder for the neural spike counts and compare it with PCA at the same latent dimensions. This would let me test whether a model designed for count data preserves more of the local structure.
