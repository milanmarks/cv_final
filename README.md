# cv_final
it's a repository for my computer vision final project

- june 2 2021: set up the baseline

## baseline study
In the begining, we use a pure ViT model for baseline. We set the model parameters as below:
- patch_size = 4, which means that we cut the original image, a 3 by 32 by 32 RGB image, into 3 by 4 by 4 little image patch. In other word, each image was cut to 64 little patch, 
- dim = 128, which means that after cutting the image to 64 patch, we stretch them and project them linearly to 128 dimensional embedddings.
- depth = 12, which means there are 12 attention layers in the encoder.
- heads = 8, which means that the number of heads of attention layers is 8.
- mlp_dim = 256, which means that in the attention layer, after the attention operation, we pour the output into a MLP layer, which consist of two simple linear transformations, and the hidden dimension is 256.
- dropout = 0.1, drop out rate for encoder. To be explicit, for both attention layers and feed forward layers. 
- emb_dropout = 0, drop out rate for input embeddings.
  
