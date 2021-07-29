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

<a href="https://github.com/google/trax" target="_blank">Trax</a> is an end-to-end library for deep learning that focuses on clear code and speed. It is actively used and maintained in the Google Brain team. It is faster than Tensorflow and Pytorch and also the codes are more clear. It also supprts both TPUs and GPUs.

## Dataset

The model is trained on the famous persian poetry book of <a href="https://en.wikipedia.org/wiki/Hafez" target="_blank">The Divan of Hafez</a> by Ḥāfeẓ-e Shīrāzī, who was a Persian poet whose collected works are regarded by many Iranians as a pinnacle of Persian literature. The all his poets are inside the file named 'all_ghazals.txt'. There are around 450 poets. The pre-processing of the poets are described inside the codes. 


## Goal
### How much a neural network can learn to generate some text similar to persian poets written by Hafez.Let's give it a try, sounds fun :)

## Instructions

You can train the model from scrath using the Google Colab notebook named `Neural-text-Generation.ipynb`

## Results

I trained the model for about 2-3 hours on a GPU for 30 epochs and the model has learned to some extend the style of Hafez for writting poets. 

Some of the examle poems are:

- لنگر شيرين و بيماری هجر تو زد از نفس 
- رحم اگر چه و سوخته دل راه و نگار
- شب جگر دهد در شمش حافظ ای صبح
- زقد عشق تو هيچ رو نه خال تو بست
- با يار مفلس شراب آلوده
- وين بشنويد رندان پاکداريم

(You can take Fale Hazef using the model now HAHA)
