#Multilingual Named Entity Recognition (NER) with XLM-Roberta

This repository contains a fine-tuned XLM-Roberta model for Named Entity Recognition (NER) tasks in four languages: German (de), French (fr), Italian (it), and English (en). This project explores cross-lingual transfer learning, enabling the model to recognize named entities across multiple languages, improving language-agnostic performance.

#Project Overview

This project utilizes the xtreme dataset's PAN-X subset to fine-tune the XLM-Roberta model on multilingual NER tasks. The goal is to create a model capable of recognizing entities (such as names of persons, organizations, and locations) in multiple languages, leveraging both language-specific and cross-lingual NER capabilities.

#Features

Multilingual Support: Trained on German, French, Italian, and English, with consistent F1-scores across languages.
Cross-Lingual Transfer: Evaluated cross-lingual transfer by training on one language and testing on another.
Error Analysis: Comprehensive error analysis through token-level loss tracking, confusion matrix visualizations, and predictions inspection.
Dynamic Training Pipeline: Fine-tuned on different dataset sizes to analyze performance progression and identify optimal training data requirements.
