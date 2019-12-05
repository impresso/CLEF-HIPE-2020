---
layout: page
title: About
order: 0
image: '/images/pages/project-schema.jpg'
---

HIPE is a named entity processing evaluation campaign on historical newspapers in French, German and English, organized in the context of the [_impresso_](http://impresso-project.ch) project and run as a [CLEF 2020](https://clef2020.clef-initiative.eu/) Evaluation Lab. In the context of massive digitization of historical documents, the objective is to assess and advance the development of robust named entity processing systems able to deal with challenging, multilingual, diachronic historical material, thereby supporting information extraction and text understanding of cultural heritage data.

### Tasks

#### Task 1: Named Entity Recognition and Classification (NERC)

- **Subtask 1.1 - NERC Essentials**: this task includes the recognition and classification of high-
level entity types: Person, Organisation, Location and Product.
- **Subtask 1.2 - NERC fine-grained**: includes ‘NERC Essentials’, plus the detection and classification at sub-type level (e.g. Person-individual vs. Person-collective) and the detection of NE components (e.g. function, title, name).

#### Task 2 : Named Entity Linking (EL)

- **Subtask 2.1 - Entity coreference resolution**: given a set of mentions, cluster them into coreferent sets and give them a unique identifier.
- **Subtask 2.2 - Entity Linking**: this task includes the linking of named entity mentions to a unique referent in a knowledge base (KB) or to a NIL node if the mention does not have a referent in the KB. The chosen KB is [Wikidata](https://wikidata.org).
