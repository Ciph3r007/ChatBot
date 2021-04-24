# ChatBot
A chatbot trained using the Reformer model. Trained on the MultiWoz Dialogue dataset.

Trained using [TRAX](https://github.com/google/trax): An end-to-end library for Deep Learning that focuses on clear code and speed. It is actively used and maintained in the Google Brain team.

## Dataset
The MultiWoz dataset consists of more than 10k dialogues within some fixed domains. Besides dialogues it contains many metadata for other research purposes. More details are available on the readme file of the dataset.

This dataset is open-source and can be downloaded from [here](https://www.repository.cam.ac.uk/handle/1810/280608).

## Model Overview
The Reformer model is a modified Transformer built to tackle some challenges of the Transformer model. Instead of paying attention to all of the input sequence, Reformer uses Locality Sensitive Hashing to focus on a much lower portion of the inputs to calculate attention. It also uses reversible residual blocks or RevNets to calculate activations only once, which are sufficent for backpropagation.

## Results
The chatbot model need much more tuning and training. But it can still grasp the content of the dialogue and generates sentences with syntax preservation more often than not.
