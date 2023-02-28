[![License: GPL v3](https://img.shields.io/badge/License-GNU-blue)](https://github.com/dezzai/Spanish-BFF/blob/main/LICENSE)
# Spanish-BFF

Avaliable in Hugging Face https://huggingface.co/datasets/MMG/SpanishBFF

## Dataset Description

Spanish-BFF is the first Spanish AI-generated dictionary using GPT3.

- **Paper:** [Spanish Built Factual Freectianary (Spanish-BFF): the first IA-generated free dictionary](https://arxiv.org/abs/2302.12746)
- **Point of Contact:** oscar.garcia@dezzai.com , alfonso.ardoiz@dezzai.com


### Dataset Summary

Spanish-BFF contains a total of 66353 lemmas with its definitions (only one definiton per lemma).

These lemmas correspond to nominal, adjetival, verbal and adverbial classes.


### Languages

- Spanish (es)


## Dataset Structure

### Data Instances

<pre>
{
'id': 'b0o8', 
'lemma': 'fomo', 
'definition': 'FOMO es un acrónimo de "miedo a perderse", y se refiere a la ansiedad que uno puede sentir cuando ve que otros están disfrutando de algo que él o ella no está haciendo.', 
}
</pre>

### Data Fields

<pre>
{
  id: str
  lemma: str
  difinition: str
}
</pre>

### Data Splits

| Split | Size |
| ------------- | ------------- |
| `train` | 66,353 |


## Content analysis

### Number of nouns, adjetives, adverbs and verbs

* Number of nouns: ???
* Number of adjetives: ???
* Number of adverbs: ???
* Number of verbs: ???


### Stadistics of tokens

* Total tokens in definitions: ???
* Average tokens/definition: ???


## Dataset Creation

### Prompting

Each one of the definitons were generated in batches using the following prompt:
<pre>
Generate in Spanish a definition of the word "[word]"
</pre>

## Considerations for Using the Data

### Social Impact of Dataset

This corpus is the first open-source complete dictionary produced by LLMs. We intend to contribute to a better un-
derstanding and development of NLP and promote responsible use. 

### Biases and Hallucinations

This version have been not postprocessed to mitigate potential errors, biases or hallucinations the IA model could have generated.


## Citation 

```
@misc{https://doi.org/10.48550/arxiv.2302.12746,
  doi = {10.48550/ARXIV.2302.12746},
  
  url = {https://arxiv.org/abs/2302.12746},
  
  author = {Sierra, Óscar García and Ortega-Martín, Miguel and Ardoiz, Alfonso and Armenteros, Juan Carlos and Álvarez, Jorge and Alonso, Adrián},
  
  keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
  
  title = {Spanish Built Factual Freectianary (Spanish-BFF): the first IA-generated free dictionary},
  
  publisher = {arXiv},
  
  year = {2023},
  
  copyright = {Creative Commons Attribution 4.0 International}
}
```