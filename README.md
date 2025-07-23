**Multilingual Named Entity Recognition (NER) with XLM-Roberta**

This portfolio project demonstrates the fine-tuning of the XLM-Roberta model for Named Entity Recognition (NER) tasks across four languages: German (de), French (fr), Italian (it), and English (en). The project's primary focus is on cross-lingual transfer learning, which allows the model to recognize named entities in multiple languages, thereby enhancing its language-agnostic performance.

**Project Overview**

This project employs the PAN-X subset of the xtreme dataset to fine-tune the XLM-Roberta model for multilingual NER tasks. The objective is to develop a model that can identify entities (such as names of persons, organizations, and locations) in various languages, capitalizing on both language-specific and cross-lingual NER capabilities.

**Data**

The PAN-X subset of the xtreme dataset used in this project comprises training, validation, and test datasets. Each dataset includes features such as 'tokens', 'ner_tags', and 'langs'. The training dataset consists of 20,000 rows, while the validation and test datasets each contain 10,000 rows.

**Approach**

The project approach involves training the model on German, French, Italian, and English datasets, evaluating its cross-lingual transfer capabilities by training on one language and testing on another. It also includes a comprehensive error analysis through token-level loss tracking, confusion matrix visualizations, and predictions inspection. The model is fine-tuned on different dataset sizes to analyze performance progression and identify optimal training data requirements.

**Findings**

The model demonstrates multilingual support with consistent F1-scores across all four languages. The cross-lingual transfer learning approach has proven effective, with the model showing robust performance even when trained on one language and tested on another. The error analysis and dynamic training pipeline provide valuable insights into the model's performance and the optimal training data requirements.

**Reproducibility**

To reproduce the results, you will need to install the following Python packages: pandas, datasets, and collections. The code can be executed in a Jupyter notebook environment. The dataset can be loaded using the 'load_dataset' function from the 'datasets' package with 'xtreme' as the dataset and 'PAN-X.de' as the name.