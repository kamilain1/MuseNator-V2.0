# MuseNator-V2.0
MuseNator version 2, implemented using GPT-2 Transformer architecture

Full kernel with dataset and outputs available here: https://www.kaggle.com/code/kamilain/musenator-v2-0-gpt2

## Details:
MuseNator is able to generate music similar to one it was trained on. In the second version, LSTM was replaced by GPT-2, which improved overall performance, since transformers are able to "remember" longer sequences and relations between previous timesteps. 

## Tools and libraries:
- TensorFlow
- HuggingFace Transformers
- pretty-midi

## Dataset:
Over 80 Mozart pieces of Maestro dataset. The decision to reduce number of training samples is due to long training time. Also, when training on pieces different piano composers, style of generated music was becoming mixed.

## Results and further changes:
Currently model generalizes given data quite well, however fixed length of notes gives synthetic and not very pleasant listening experience. Further improvements will cover varying note duration and step. Also I would like to reimplement the pipeline using PyTorch.
