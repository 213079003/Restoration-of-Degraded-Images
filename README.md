# Patchwise Denoising of Synthetically Degraded Images 
Using a patch-based methodology, this notebook provides code for picture denoising.Initially, clean images of BSDS300 dataset are taken and these images are degraded with gaussian blurring with kernel size of 5x5 and salt and pepper noise with an amout of 0.2. Patches of size 27x27 are extracted from each of these images, and the target being the central pixels of the clean patches. These degraded patches are given as an input to the Deep Neural Network, and three regression outputs are obtained (R, G, B pixel values) which denote the predicted central pixel.
This model achieved an MSE loss of **0.0285** on validation set.


# Dataset Used: 
- BSDS300 : [LINK](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/)
