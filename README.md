# ExploreAI Academy Classification Hackathon
This repository contains the notebook for the ExploreAI Academy Classification Hackathon, which focuses on language identification for South Africa's 11 official languages. The objective is to identify the language of a given text, leveraging natural language processing techniques.

## Overview
South Africa is known for its rich linguistic diversity, with 11 official languages. Language plays a crucial role in the country's social, cultural, economic, and political life. With a multilingual population, it becomes essential to develop systems and devices that can effectively communicate in multiple languages.

The challenge in this hackathon is to determine the language of a given text written in any of South Africa's official languages. This task is a form of language identification in the field of natural language processing (NLP).

## Evaluation Metric
The evaluation metric for this competition is the Mean F1-Score. The F1 score, commonly used in information retrieval, combines the precision and recall statistics to measure accuracy. Precision is the ratio of true positives (tp) to all predicted positives (tp + fp), while recall is the ratio of true positives to all actual positives (tp + fn). The F1 score is calculated as follows:


The F1 score is calculated using the formula:

$$ F1 = \frac{2 \cdot (precision \cdot recall)}{precision + recall} $$


The F1 metric equally weighs precision and recall, favoring models that achieve a balanced performance on both metrics.

#### Submission Format
The submission file should be in CSV format and contain the following columns:

index: The index of the dataset entry.
lang_id: The language tag of the predicted language.
The submission file should have a header row, and each row should correspond to a unique index in the dataset.

## Cloning the repo
```
git clone https://github.com/VaporFoxLash/LanguageIdentifier
```

## Libraries and Installation
To run this notebook, the following libraries are required:

numpy: A library for numerical computing in Python.
pandas: A library for data manipulation and analysis.
scikit-learn: A machine learning library for Python.
nltk: A natural language processing library for Python.
tensorflow: An open-source deep learning framework.
You can install these libraries by running the following command in your terminal:

```
pip install numpy pandas scikit-learn nltk
```

Note: If you have a requirements file in this directory/repository, you can install all the necessary libraries by running the following command:
```
pip install -r requirements.txt
```

## Usage
Install the required libraries using the provided installation instructions.
Ensure that the dataset and necessary files are accessible in the appropriate paths or directories.
Run the notebook cells sequentially to train models, perform evaluations, and generate predictions.
Adjust the hyperparameters, feature selection, or model architecture as needed.
