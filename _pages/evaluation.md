---
layout: page
title: Evaluation settings
order: 30
#image: 'images/pages/scorer.jpg'
---



**Scorers**

HIPE scorer available **[HERE](https://github.com/impresso/CLEF-HIPE-2020-scorer)**.

**Metrics**

**NERC** is evaluated in terms of **macro and micro Precision, Recall, F1-measure**. Two evaluation scenarios are considered: **strict** (exact boundary matching) and **relaxed** (fuzzy boundary matching). 

Each column is evaluated independently, according to the following metrics:

- Micro average P, R, F1 at entity level (not at token level), i.e. consideration of all true positives, false positives, true negatives and false negative over all documents. 
  - strict (exact boundary matching) and fuzzy (at least 1 token overlap).
  - separately per type and cumulative for all types.
  
- Document-level macro average P, R, F1 at entity level (not on token level). i.e. average of separate micro evaluation on each individual document.
  - strict and fuzzy
  - separately per type and cumulative for all types
  

Our definition of macro differs from the usual one, and macro measures are computed as aggregates on document-level instead of entity-type level. Specifically, macro measures average the corresponding micro scores across all the documents, accounting for (historical) variance in document length and not for class imbalances.

Note that in the strict scenario, predicting wrong boundaries leads to severe punishment of one false negative (entity present in the gold standard but not predicted by the system) and one false positive (predicted entity by the system but not present in the gold standard). Although this may be severe, we keep this metric in line with [CoNLL](https://www.clips.uantwerpen.be/conll2000/chunking/output.html) and refer to the fuzzy scenario if the boundaries of an entity are considered as less important.

The Slot Error Rate (SER) is dropped for the shared task evaluation.

The evaluation for **NEL** works similarly as for NERC. The link of an entity is interpreted as a label. As there is no IOB-tagging, a consecutive row of identical links is considered as a single entity. In terms of boundaries, NEL is only evaluated according to the fuzzy scenario. Thus, to get counted as correct, the system response needs only one overlapping link label with the gold standard. 

[TODO: potentially add a word on fuzzy (= more than one link) NEL evaluation]





