---
layout: page
title: Data
order: 20
#image: 'images/pages/corpora.jpg'
---



The shared tasks corpora are composed of articles sampled among several Swiss, Luxembourgish and American historical newspapers on a diachronic basis.

Data acquisition and format are described in the [HIPE - Shared Task Participation Guidelines](https://zenodo.org/record/3677171).

#### Data sets:

- **Sample data** for French and German is available **[HERE](https://github.com/impresso/CLEF-HIPE-2020/tree/2020-01-10/data/)**. It consists of 10 French and 8 German content items fully annotated.
- **Training and dev data sets** (all versions) are available **[HERE](https://github.com/impresso/CLEF-HIPE-2020/tree/master/data)**. See statistics below.



#### Auxiliary resources
HIPE provides several **‘in domain’ embeddings** acquired from the impresso newspapers and time periods from which HIPE training and development sets were extracted.

***We strongly encourage participants to also share any external resource they might use, during and/or after the evaluation campaign.***



- **fasttext word embeddings**

We offer fasttext word embeddings without subwords ([link](https://files.ifi.uzh.ch/cl/siclemat/impresso/clef-hipe-2020/fasttext/fr-model-skipgram-300minc20-ws5-maxn-0.bin)) and with subword 3-6 character n-grams ([link](https://files.ifi.uzh.ch/cl/siclemat/impresso/clef-hipe-2020/fasttext/fr-model-skipgram-300minc20-ws5-maxn-6.bin)). Additionally to the binary models, we uploaded textual .vec formats. For all downloads, follow this [link](https://files.ifi.uzh.ch/cl/siclemat/impresso/clef-hipe-2020/fasttext/).

The preprocessing tries to mimic the tokenization of the HIPE data and involves the following normalizations: lowercasing; replacement of each digit by 0; deletion of all tokens with length 1 (e.g. punctuation).

 The exact training parameters of each model `MODEL.bin` can be found in  the corresponding file `MODEL.bin.info.txt` as computed by the  `fasttext dump args`.

 For more information on fasttext and tutorials, visit [the fasttext website](https://fasttext.cc).



- **flair contextualized string embeddings (aka. character embeddings)**

For download, visit this [link](https://files.ifi.uzh.ch/cl/siclemat/impresso/clef-hipe-2020/flair). You will find the forward and backward model for each language in a separate directory: `best-lm.pt` contains the parameters you will use and `loss.txt` contains the training logs (scores on the training and dev set).

The preprocessing involves the following steps: lowercasing; replacement of each digit by 0; replacement of each newline by space. Everything else was kept as in the original text (e.g. tokens of length 1). 

Here is an example of the input to flair:

```
in . the mer- chant's, family was lost sight of. it was doubtless destroyed more than a cen- tury ago. liut not so with tatty, the pet of the parsonage. abigail french, the minis- ter's daughter, w
as born on the last day of may, 0000. she was eight years of age when she received this treasure. mrs`
```





The amount for our our in-domain training differs largely between languages: French taken from Swiss and Luxembourgish newspapers: 20G; English taken from Chronicling America material: 1.1G; German taken from Swiss and Luxembourgish newspapers: 8.5G.

The embedding size for characters is 2048. We use flair 0.4.5 to compute the embeddings using a context of 250 characters, a batchsize of 400-600 (depending on the GPUs memory), 1 hidden layer, dropout of 0.1. See the [tutorial on language modeling](https://github.com/flairNLP/flair/blob/master/resources/docs/TUTORIAL_9_TRAINING_LM_EMBEDDINGS.md) for more information.

For more information on flair and tutorials on how to use flair embeddings, visit [the flair website](https://github.com/flairNLP/flair). 

***We strongly encourage participants to also share any external resource they might use, during and/or after the evaluation campaign.***



 <a href="#top">Back to top</a>



#### Statistics about HIPE data release v1.2

Computed on version `v1.02` of our datasets;  last update: 12 May 2020.



**Overview**

![alt](images/pages/overview-table-12May2020.png)

As a reminder, we are not releasing training data for English.



**Number of documents by decade**

![alt](images/pages/n_documents_diachronic-12May2020.png)



**Number of tokens by decade**

![alt](images/pages/n_tokens_diachronic-12May2020.png)	



**Number of mentions by decade**

![alt](images/pages/n_mentions_diachronic-12May2020.png)



**Number of mentions, broken down by type (coarse)**

![alt](images/pages/coarse-12May2020.png)



**Number of mentions by decade, broken down by type (coarse)**

![alt](images/pages/coarse_types_diachronic-12May2020.png)



**NIL entities ratio**

Number of NIL entities over the total number of mentions (per decade).

![alt](images/pages/nil_ratio_diachronic-12May2020.png)



**NIL entities by mention type (coarse)**

![alt](images/pages/coarse_nil-12May2020.png)



**Metonymy**

![alt](images/pages/mentonymy_diachronic-12May2020.png)

![alt](images/pages/mentonymy_by_language_diachronic-12May2020.png)



 <a href="#top">Back to top</a>



#### Statistics about HIPE data release v1.1 

No statistics, data very similar to v1.0



#### Statistics about HIPE data release v1.0 

Computed on version `v1.0` of our datasets;  last update: 26 March 2020.



**Overview**

![alt](images/pages/overview-table-26March2020.png)

As a reminder, we are not releasing training data for English.



**Number of documents by decade**

![alt](images/pages/n_documents_diachronic-26March2020.png)



**Number of tokens by decade**

![alt](images/pages/n_tokens_diachronic-26March2020.png)	



**Number of mentions by decade**

![alt](images/pages/n_mentions_diachronic-26March2020.png)



**Number of mentions, broken down by type (coarse)**

![alt](images/pages/coarse-26March2020.png)



**Number of mentions by decade, broken down by type (coarse)**

![alt](images/pages/coarse_types_diachronic-26March2020.png)



**NIL entities ratio**

Number of NIL entities over the total number of mentions (per decade).

![alt](images/pages/nil_ratio_diachronic-26March2020.png)



**NIL entities by mention type (coarse)**

![alt](images/pages/coarse_nil-26March2020.png)



**Metonymy**

![alt](images/pages/mentonymy_diachronic-26March2020.png)

![alt](images/pages/mentonymy_by_language_diachronic-26March2020.png)



 <a href="#top">Back to top</a>



### Statistics about HIPE data release v0.9 

Computed on version `v0.9` of our datasets;  last update: 20 February 2020.



**Overview**

![alt](images/pages/overview-table-20Feb2020.png)

As a reminder, we are not releasing training data for English.



**Number of documents by decade**

![alt](images/pages/n_documents_diachronic-20Feb2020.png)



**Number of tokens by decade**

![alt](images/pages/n_tokens_diachronic-20Feb2020.png)	



**Number of mentions by decade**

![alt](images/pages/n_mentions_diachronic-20Feb2020.png)



**Number of mentions, broken down by type (coarse)**

![alt](images/pages/coarse-20Feb2020.png)



**Number of mentions by decade, broken down by type (coarse)**

![alt](images/pages/coarse_types_diachronic-20Feb2020.png)



**Average number of NIL entities per document**

We link mentions against Wikidata. NIL entities are those that do not have a corresponding entry in Wikidata.

![alt](images/pages/avg_nil-entities_diachronic-20Feb2020.png)



**NIL entities ratio**

Number of NIL entities over the total number of mentions (per decade).

![alt](images/pages/nil_ratio_diachronic-20Feb2020.png)



**NIL entities by mention type (coarse)**

![alt](images/pages/coarse_nil-20Feb2020.png)

**Metonymy**

![alt](images/pages/mentonymy_diachronic-20Feb2020.png)

![alt](images/pages/mentonymy_by_language_diachronic-20Feb2020.png)



 <a href="#top">Back to top</a>