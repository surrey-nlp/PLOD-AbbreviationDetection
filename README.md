<p align="center"><img src="./imgs/plod.png" alt="logo" width="65" height="100"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="imgs/faviconcts-logo.png" alt="logo" width="185" height="100"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="imgs/aisurrey.svg" alt="logo" width="200" height="100"/></p>

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

1. The Filtered version can be accessed via [Huggingface Datasets here](https://huggingface.co/datasets/surrey-nlp/PLOD-filtered) and a CONLL format is present here in the data folder.<br/>

2. The Unfiltered version can be accessed via [Huggingface Datasets here](https://huggingface.co/datasets/surrey-nlp/PLOD-unfiltered) and a CONLL format is present here in the data folder.<br/>

3. The [SDU Shared Task](https://sites.google.com/view/sdu-aaai22/home) data we use for zero-shot testing is [available here](https://github.com/amirveyseh/AAAI-22-SDU-shared-task-1-AE).

### Installation

We use the custom NER pipeline in the [spaCy transformers](https://spacy.io/universe/project/spacy-transformers) library to train our models. This library supports training via any pre-trained language models available at the :rocket: [HuggingFace repository](https://huggingface.co/).<br/>
Please see the instructions at these websites to setup your own custom training with our dataset to reproduce the experiments using Spacy.

OR<br/>

However, you can also reproduce the experiments via the Python notebook we [provide here](https://github.com/surrey-nlp/PLOD-AbbreviationDetection/blob/main/nbs/fine_tuning_abbr_det.ipynb) which uses HuggingFace Trainer class to perform the same experiments. The exact hyperparameters can be obtained from the models readme cards linked below. Before starting, please perform the following steps:

```bash
git clone https://github.com/surrey-nlp/PLOD-AbbreviationDetection
cd PLOD-AbbreviationDetection
pip install -r requirements.txt
```

Now, you can use the notebook to reproduce the experiments.

### Model(s)


Our best performing models are hosted on the HuggingFace models repository

| Models | [`PLOD - Unfiltered`](https://huggingface.co/datasets/surrey-nlp/PLOD-unfiltered) | [`PLOD - Filtered`](https://huggingface.co/datasets/surrey-nlp/PLOD-filtered) | Description |
| --- | :---: | :---: | --- |
| [RoBERTa<sub>large</sub>](https://huggingface.co/roberta-large) | [RoBERTa<sub>large</sub>-finetuned-abbr](https://huggingface.co/surrey-nlp/roberta-large-finetuned-abbr) | -soon- | Fine-tuning on the RoBERTa<sub>large</sub> language model |
| [RoBERTa<sub>base</sub>](https://huggingface.co/roberta-base) | -soon- | [RoBERTa<sub>base</sub>-finetuned-abbr](https://huggingface.co/surrey-nlp/roberta-large-finetuned-abbr) | Fine-tuning on the RoBERTa<sub>base</sub> language model |
| [AlBERT<sub>large-v2</sub>](https://huggingface.co/albert-large-v2) | [AlBERT<sub>large-v2</sub>-finetuned-abbDet](https://huggingface.co/surrey-nlp/albert-large-v2-finetuned-abbDet) | -soon- | Fine-tuning on the AlBERT<sub>large-v2</sub> language model |



On the link provided above, the model(s) can be used with the help of the Inference API via the web-browser itself. We have placed some examples with the API for testing.<br/>

### Usage

You can use the HuggingFace Model link above to find the instructions for using this model in Python locally using the notebook provided in the Git repo. 

## Citing

Please use the following citation while citing this work:

```latex
@misc{https://doi.org/10.48550/arxiv.2204.12061,
  doi = {10.48550/ARXIV.2204.12061},
  url = {https://arxiv.org/abs/2204.12061},
  author = {Zilio, Leonardo and Saadany, Hadeel and Sharma, Prashant and Kanojia, Diptesh and Orasan, Constantin},
  keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {PLOD: An Abbreviation Detection Dataset for Scientific Documents},
  publisher = {arXiv},
  year = {2022},
  copyright = {Creative Commons Attribution 4.0 International}
}
```

## Maintainer(s)

[Diptesh Kanojia](https://dipteshkanojia.github.io) <br/>
[Prashant Sharma](http://prashantksharma.com/) <br/>



