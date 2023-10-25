<div align="center">
<img src="https://github.com/artnoage/Experimental-Llama/blob/main/llama.png" width="400">
</div>


The purpose of this repo is to play around with different architectures. 

This is a fork from the repo https://github.com/jzhang38/TinyLlama. I made some minor quality of life changes borrowed by Karpathy's llama.c repo (https://https://github.com/karpathy/llama2.c). Changes include the following:
I corrected the formula of how intermidiate_dim is calculated. Also the number of groups for the 120M network. 

I also tighted the weights of head and embed layer.

Remark about speed: Playing around with small models (up to 160M), I noticed that Karpathy's implementation is faster due to compilation of the model. This conflicts with the latest vesion of flash-attention.
