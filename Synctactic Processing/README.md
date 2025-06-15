# Identifying Entities in Healthcare Data
> Develop a custom Named Entity Recognition (NER) system to extract and categorize diseases and their corresponding treatments from medical text data.


## Table of Contents :
* [Problem Statement](#problem-statement)
* [Objectives](#objectives)
* [Approach](#approach)
* [Technologies/Libraries Used](#technologies/libraries-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Glossary](#glossary)
* [Author](#author)


## Problem Statement
Let’s consider a hypothetical example of a health tech company called ‘BeHealthy’. Suppose ‘BeHealthy’ aims to connect the medical communities with millions of patients across the country. 

‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.
So, companies like ‘BeHealthy’ are providing medical services, prescriptions and online consultations and generating huge data day by day.
Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.

“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”
As you can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’. 

Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.

But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you can build an algorithm to map the diseases and their respective treatment.

Suppose you have been asked to determine the disease name and its probable treatment from the dataset and list it out in the form of a table or a dictionary like this. 
After discussing the problem given above, you need to build a custom NER to get the list of diseases and their treatment from the dataset.

Download the dataset given below.

[Train Sentence Dataset]( https://github.com/arnabberawork/Syntactic-Processing-Assignment/blob/main/train_sent )

[Train Label Dataset]( https://github.com/arnabberawork/Syntactic-Processing-Assignment/blob/main/train_label )

[Test Sentence Dataset]( https://github.com/arnabberawork/Syntactic-Processing-Assignment/blob/main/test_sent )

[Test Label Dataset]( https://github.com/arnabberawork/Syntactic-Processing-Assignment/blob/main/test_label )

Here, you need to understand that each word in this dataset is provided in a single line. So, first, you need to club all these words together to form the sentences. Moreover, there are blank lines given in the dataset that have been highlighted in the image given above. These blank lines indicate that a new sentence is starting from the next line onwards to the next blank line.

## Objectives
The objective of this project is to build a custom Named Entity Recognition (NER) model that can extract and categorize diseases and their associated treatments from unstructured medical text data. The solution should:

- You need to process and modify the data into sentence format. This step has to be done for the 'train_sent' and ‘train_label’ datasets and for test datasets as well.
- After that, you need to define the features to build the CRF model.
- Then, you need to apply these features in each sentence of the train and the test dataset to get the feature values.
- Once the features are computed, you need to define the target variable and then build the CRF model.
- Then, you need to perform the evaluation using a test data set.
- After that, you need to create a dictionary in which diseases are keys and treatments are values.

## Approach

- Step 1: Workspace set up: Import and Install Necessary Libraries
- Step 2: Load the Data and Understanding the Data
- Step 3: Data Preparation Steps - construct the proper sentences from individual words 
- Step 4: Concept Identification - Exploratory Data Analysis
- Step 5: Defining features for CRF
- Step 6: Define input and target variables
- Step 7: Build the CRF Model
- Step 8: Evaluation
- Step 9: Making Predictions Using the Model
  
## Technologies/Libraries Used
- Python: 3.12.3 | packaged by conda-forge | (main, Apr 15 2024, 18:20:11) [MSC v.1938 64 bit (AMD64)]
- NumPy: 1.26.4
- Pandas: 2.2.2
- Spacy: 3.8.2

## Conclusions
In this project, two models were developed to extract diseases and treatments from unstructured medical text:

Model 1 (Using POS as a feature): Achieved an F1 score of 0.907.

Model 2 (Using both POS and Dependency Parsing as features): Achieved an F1 score of 0.904.

Both models performed well, with Model 1 slightly outperforming Model 2. The use of POS tagging and dependency parsing as features contributed positively to the extraction process, demonstrating the effectiveness of these linguistic features in improving NER performance.

Further Steps/Improvements:

To enhance the model further, consider exploring the following:

Additional Features: Experiment with adding other features such as word embeddings (e.g., Word2Vec, GloVe) or character-level features (e.g., character n-grams) to capture more semantic information.

Deep Learning Models: Try using more advanced deep learning-based NER models like BERT or BioBERT, which are specifically designed for medical text and might improve accuracy.

Entity Linking: Add a post-processing step for linking the extracted entities to a medical knowledge base (e.g., UMLS) for better contextual understanding.

## Acknowledgements

- The project reference course materieals from upGrads curriculm .
- The project references from presentation in upGrads module given by [Sumit Bhatia](https://www.linkedin.com/in/sumitonlinkedin/)
- The project references from presentation in upGrads live class given by [Shivam Garg](https://www.linkedin.com/in/shivam-garg-0494a2ab/)
- The project references insights and inferences from presentation in upGrads live class given by [Tanisha Medewala](https://www.linkedin.com/in/tanishamedewala/)

## Glossary

- Exploratory Data Analysis (EDA)
- Feature Engineering
- Tokenization
- Sequence Labeling
- F1 Score
- Training Data and Test Data
- spaCy
- Token Embeddings
- Part-of-Speech (POS) Tagging
- Dependency Parsing
- Named Entity Recognition (NER)
- Conditional Random Fields (CRF)
- CRFsuite
- Custom Feature Function

## Author
* [Arnab Bera]( https://www.linkedin.com/in/arnabbera-tech/ )
