---
layout: page
title: Data
order: 20
#image: 'images/pages/corpora.jpg'
---



The shared tasks corpora are composed of articles sampled among several Swiss, Luxembourgish and American historical newspapers on a diachronic basis.

Data acquisition and format are described in the [HIPE - Shared Task Participation Guidelines]().

#### Data sets:

- **Sample data** for French and German is available **[HERE](https://github.com/impresso/CLEF-HIPE-2020/tree/2020-01-10/data/)**. It consists of 10 French and 8 German content items fully annotated.
- **Training and dev data sets** version 0.9 are available **[HERE]()**.



#### Auxiliary resources

- HIPE will provide ‘in domain’ word-level and character-level embeddings acquired from historical newspaper corpora.

- Participants will be encouraged (but not forced) to share any  external resource they might use, during and/or after the evaluation  campaign.

  

#### Statistics about HIPE data release v0.9 

- computed on version `v0.9` of our datasets;
- last updated: 20 February 2020.



**Overview**

| language | # of documents | # of tokens | # of mentions | # of entities |
| :------- | :------------- | ----------- | ------------- | ------------- |
| de       | 106            | 68967       | 5293          | 5293          |
| fr       | 120            | 91801       | 7771          | 7771          |
| en       | 108            | 33579       | 1284          | 1284          |

As a reminder, we are not releasing training data for English.



**Number of documents by decade**

![](CLEF-HIPE-2020/images/pages/n_documents_diachronic.png)



**Number of tokens by decade**

![](CLEF-HIPE-2020/images/pages/n_tokens_diachronic.png)	



**Number of mentions by decade**

![](CLEF-HIPE-2020/images/pages/n_mentions_diachronic.png)



**Number of mentions, broken down by type (coarse)**

| coarse type | of mentions |
| :---------- | ----------: |
| loc         |        4878 |
| org         |        1861 |
| pers        |        3387 |
| prod        |         269 |
| time        |         337 |

**Number of mentions by decade, broken down by type (coarse)**

![](CLEF-HIPE-2020/images/pages/coarse_types_diachronic.png)



**Average number of NIL entities per document**

We link mentions against Wikidata. NIL entities are those that do not have a corresponding entry in Wikidata.

![](CLEF-HIPE-2020/images/pages/avg_nil-entities_diachronic.png)



**NIL entities ratio**

Number of NIL entities over the total number of mentions (per decade).

![](CLEF-HIPE-2020/images/pages/nil_ratio_diachronic.png)



**NIL entities by mention type (coarse)**

| coarse type | # of NIL entities |
| :---------- | ----------------: |
| pers        |              1410 |
| org         |               357 |
| loc         |               229 |

**Metonymy**

![](CLEF-HIPE-2020/images/pages/mentonymy_diachronic.png)

![](CLEF-HIPE-2020/images/pages/mentonymy_by_language_diachronic.png)