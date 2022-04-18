<p align="center"><img src="./imgs/plod.png" alt="logo" width="50" height="84"/></p>

# PLOD: An Abbreviation Detection Dataset  
[![GitHub issues](https://img.shields.io/github/issues/surrey-nlp/PLOD-AbbreviationDetection?style=flat-square)](https://github.com/surrey-nlp/PLOD-AbbreviationDetection/issues)
[![GitHub stars](https://img.shields.io/github/stars/surrey-nlp/PLOD-AbbreviationDetection?style=flat-square)](https://github.com/surrey-nlp/PLOD-AbbreviationDetection/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/surrey-nlp/PLOD-AbbreviationDetection?style=flat-square)](https://github.com/surrey-nlp/PLOD-AbbreviationDetection/network)
[![GitHub license](https://img.shields.io/github/license/surrey-nlp/PLOD-AbbreviationDetection?style=flat-square)](https://github.com/surrey-nlp/PLOD-AbbreviationDetection)
[![Twitter Follow](https://img.shields.io/twitter/follow/CTS_Surrey?color=1DA1F2&logo=twitter&style=flat-square)](https://twitter.com/CTS_Surrey)
[![Twitter Follow](https://img.shields.io/twitter/follow/PeopleCentredAI?color=1DA1F2&logo=twitter&style=flat-square)](https://twitter.com/PeopleCentredAI)

This is the repository for PLOD Dataset submitted to LREC 2022. The dataset can help build sequence labelling models for the task Abbreviation Detection. 

### Dataset

We provide two variants of our dataset - Filtered and Unfiltered. They are described in our paper here.

1. The Filtered version can be accessed via [Huggingface Datasets here](https://huggingface.co/datasets/surrey-nlp/PLOD-filtered) and a [CONLL format is present here](https://github.com/surrey-nlp/PLOD-AbbreviationDetection).<br/>

2. The Unfiltered version can be accessed via [Huggingface Datasets here](https://huggingface.co/datasets/surrey-nlp/PLOD-unfiltered) and a [CONLL format is present here](https://github.com/surrey-nlp/PLOD-AbbreviationDetection).<br/>

3. The [SDU Shared Task](https://sites.google.com/view/sdu-aaai22/home) data we use for zero-shot testing is [available here](https://github.com/amirveyseh/AAAI-22-SDU-shared-task-1-AE).

### Installation
We use the custom NER pipeline in the [spaCy transformers](https://spacy.io/universe/project/spacy-transformers) library to train our models. This library supports training via any pre-trained language models available at the :rocket: [HuggingFace repository](https://huggingface.co/).<br/>
Please see the instructions at these websites to setup your own custom training with our dataset.

### Model(s)
The working model is present [here at this link](https://huggingface.co/surrey-nlp/en_abbreviation_detection_roberta_lar).<br/>
On the link provided above, the model can be used with the help of the Inference API via the web-browser itself. We have placed some examples with the API for testing.<br/>

#### Usage (in Python)
You can use the HuggingFace Model link above to find the instructions for using this model in Python locally. 





