---
layout: page
title: Tasks
order: 10
#image: 'images/pages/about.jpeg'
---



### Overview 

**Task 1: Named Entity Recognition and Classification (NERC)**

- *Subtask 1.1 - NERC Coarse-grained*: this task includes the recognition and classification of entity mentions according to coarse-grained types (Person, Location, Organisation and Product).
- *Subtask 1.2 - NERC Fine-grained*: this task includes the recognition and classification of entity mentions according to fine-grained types (cf. column 2 in Table 2), plus the detection and classification of nested entities of depth 1, as well as entity mention components.

**Task 2 : Named Entity Linking (EL)**

This task includes the linking of named entity mentions to a unique referent in a knowledge base (KB) or to a NIL node if the mention does not have a referent in the KB. The chosen KB is [Wikidata](https://wikidata.org).

The entity linking task includes two settings: with and without prior knowledge of mention boundaries. Concretely speaking, the [evaluation period](dates.html) will consist of two consecutive rounds, where a first NEL task without prior information on mentions will be evaluated during round 1 (i.e. task bundles 1 and 2), and a second one with information on mention boundaries (but no type) during the second round (bundle 5).



### Detailed description

For a detailed description of the tasks and instructions relative to participation, download the **[HIPE - Shared Task Participation Guidelines](https://zenodo.org/record/3604238).**



### Task bundles

| **Bundle id** | **Associated tasks**              | **Relevant columns in the IOB response file**                |
| ------------- | --------------------------------- | ------------------------------------------------------------ |
| bundle 1      | NERC-coarse and NERC-fine and NEL | TOKEN, NE-COARSE, NE-FINE-LIT, NE-FINE-METO, NE-FINE-COMP, NE-FINE-NESTED, NEL |
| bundle 2      | NERC-coarse and NEL               | TOKEN, NE-COARSE, NEL                                        |
| bundle 3      | NERC-coarse and NERC-fine         | TOKEN, NE-COARSE, NE-FINE1, NE-FINE1-COMP, NE-FINE2          |
| bundle 4      | NERC-coarse                       | TOKEN, NE-COARSE                                             |
| bundle 5      | NEL                               | TOKEN, NEL                                                   |

