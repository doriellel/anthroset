# anthroset

This repository contains the dataset used in the challenge set described in the paper:

**AnthroSet: a Challenge Dataset for Anthropomorphic Language Detection**  
Dorielle Lonke, Jelke Bloem and Pia Sommerauer

To be published in the proceedings of: OMMM 2025: The first Interdisciplinary Workshop on Observations of Misunderstood, Misguided and Malicious Use of Language Models (forthcoming)

## Contents

The repository includes:

- `data/`: the dataset files used in the challenge set.
- `guidelines.pdf`:: the annotation procedure and decisions.
- `README.md`: description of the dataset and usage instructions.

## Dataset Description

### Information

The challenge set contains 600 sentences from abstracts of papers on the topic of AI, published on ACL Anthology and arXiv.
The dataset consists of six linguistic categories: (1) verb subjects, (2) verb ojbects, (3) adjectives, (4), role/function noun phrases, (5), genitive noun phrases and (6) comparisons. The multiclass set of verbs and adjectives contain positive, negative and inconclusive samples. The single class set of nouns contains only positive cases, and the comparison sentences are labeled inconclusive (annotation decisions are described within the paper). 

### format and structure

The data is provided in csv format. Each csv file contains the sentence, its previous and next sentence context, its masked version, the complete noun phrase containing the AI entity, the minimal AI entity which was masked, the lemma of the AI entity, the (non-)anthropomorphic component, and the label. The labels are values in [0,1,2] corresponding to negative, positive and inconclusive judgments.
