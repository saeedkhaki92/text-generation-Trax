# text-generation-Trax
This repository contains codes for neural text generation for poem

The goal of this project is to predict predict the next set of characters using the previous characters. The used model first converts each character to its embedding, run the embeddings through a Gated Recurrent Unit GRU, and run it through a linear layer to predict the next set of characters. The RNN part of the model looks the figure below but it is trained at the character level.


![Alt Text](https://github.com/saeedkhaki92/text-generation-Trax/blob/main/pic1.png)
