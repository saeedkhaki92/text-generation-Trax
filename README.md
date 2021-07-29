# text-generation-Trax
This repository contains codes for neural text generation for poem

The goal of this project is to predict predict the next set of characters using the previous characters. The used model first converts each character to its embedding, run the embeddings through a Gated Recurrent Unit GRU, and run it through a linear layer to predict the next set of characters. The RNN part of the model looks the figure below but it is trained at the character level.


![Alt Text](https://github.com/saeedkhaki92/text-generation-Trax/blob/main/pic1.png)



## Getting Started

### Dependencies

Following packages should be installed on python 3:

- Trax
- numpy
- random



## Dataset

The model is trained on the famous persian poetry book of The Divan of Hafez by Ḥāfeẓ-e Shīrāzī, who was a Persian poet whose collected works are regarded by many Iranians as a pinnacle of Persian literature. The all his poets are inside the file named 'all_ghazals.txt'. There are around 450 poets. The pre-processing of the poets are described inside the codes. 
