# ExploreAI Academy Classification Hackathon
This repository contains the notebook for the ExploreAI Academy Classification Hackathon, which focuses on language identification for South Africa's 11 official languages. The objective is to identify the language of a given text, leveraging natural language processing techniques.

## Overview
South Africa is known for its rich linguistic diversity, with 11 official languages. Language plays a crucial role in the country's social, cultural, economic, and political life. With a multilingual population, it becomes essential to develop systems and devices that can effectively communicate in multiple languages.

The challenge in this hackathon is to determine the language of a given text written in any of South Africa's official languages. This task is a form of language identification in the field of natural language processing (NLP).

![South Africa Languages](https://github.com/VaporFoxLash/LanguageIdentifier/blob/master/assets/South_Africa_languages_2011.jpg)

[Image credit](https://bilingua.io/how-to-say-hello-in-100-languages)


## Modeling
We explore different models for language identification. We train and evaluate various models using different algorithms and techniques.


### Data Preprocessing

Before building our models, we need to preprocess the data. This involves cleaning and transforming the text data into a format suitable for modeling. The preprocessing steps include:

- **Tokenization:** Splitting the text into individual words or tokens.
- **Removing stopwords:** Removing common words that do not contribute much to the language identification task.
- **Lemmatization or stemming:** Reducing words to their base or root form.
- **Vectorization:** Converting text data into numerical feature vectors.


*Model 1:* **_Logistic Regression_**

Logistic Regression is a popular algorithm for classification tasks. It works well with linearly separable data and can provide probabilities for each class.


*Model 2:* **_Support Vector Machine (SVM)_**

Support Vector Machine is a powerful algorithm for both classification and regression tasks. It finds the best separating hyperplane to classify data into different classes.


*Model 3:* **_Radom Forest_**

Random Forest is an ensemble learning method that combines multiple decision trees to make predictions. It is known for its ability to handle complex data and reduce overfitting.


*Model 4:* **_Decision Trees_**

Decision Trees are simple yet effective models that use a tree-like structure to make decisions. Each node represents a feature, and each branch represents a decision rule.


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

- **numpy:** A library for numerical computing in Python.
- **Pandas**: A library for data manipulation and analysis.
- **scikit-learn:** A machine learning library for Python.
- **nltk:** A natural language processing library for Python.

You can install these libraries by running the following command in your terminal:

```
pip install numpy pandas scikit-learn nltk
```

To install all the necessary libraries, run the following command:
```
pip install -r requirements.txt
```

## Usage
Install the required libraries using the provided installation instructions.
Ensure that the dataset and necessary files are accessible in the appropriate paths or directories.
Run the notebook cells sequentially to train models, perform evaluations, and generate predictions.
Adjust the hyperparameters, feature selection, or model architecture as needed.


## References
https://en.wikipedia.org/wiki/Languages_of_South_Africa
https://southafrica-info.com/arts-culture/11-languages-south-africa/
https://www.ajol.info/index.php/salas
https://www.tomedes.com/translator-hub/south-africa-languages
https://www.cambridge.org/core/books/abs/language-in-south-africa/south-africa-a-sociolinguistic-overview/D79E61150FBC1CE67864320F758E799C

