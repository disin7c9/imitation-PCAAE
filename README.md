# imitation-PCAAE
A replica of PCA-AE built on a modified DeZero

## PCA-AE
PCA-AE is one of autoencoders which decomposes input data like principal component analysis (PCA), but in a non-linear way. Through the model, we can figure out the meaning of each component of the latent space of given data in statistically independent manner and manipulate the latent space intuitively. For more details, refer to the original authors' paper [1] and github code [2].

## DeZero
DeZero is one of framework for python developed by Saitou Koki. It was introduced in the 3rd volume of 'Deep learning from scratch'. You can find the official version of DeZero in the following reference [3]. I modified some classes and functions to reproduce the AE model. 
  
  In my memory, I edited
  
  class: Config, Variable, DataLoader, MeanSquaredError, BatchNorm, Linear, Conv2d, Deconv2d, Optimizer, GetItemGrad(cupy => cupyx)
    
  function: sigmoid_cross_entropy, binary_cross_entropy
  
  ... etc.
  

## References
- [1] https://link.springer.com/article/10.1007/s10851-022-01077-z
- [2] https://github.com/chieupham/PCAAE/tree/main
- [3] https://github.com/oreilly-japan/deep-learning-from-scratch-3/tree/master
