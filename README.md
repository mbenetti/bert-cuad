## Using Bert models trainned on CUAD  for contract review using Jupyter Notebooks

<img align="left" src="https://user-images.githubusercontent.com/27162948/173199085-08509c5e-ea93-4f10-8b9b-15aa143c4b1c.jpeg">


### What does contract review entail?

When it comes to contract review, a lawyer’s job is to manually review hundreds of pages of contracts to find the relevant clauses or obligations stipulated in a contract. It is repetitive because they always need to identify the same data points in any given contract: What is effective date of the contract? What are the renewal terms? Who are the parties involved in this contract?

Law firms are under enormous pressure to reduce their costs, especially during and after COVID times. With the latest advances in Natural Language Processing (NLP), machine learning models can learn to automatically extract and identify key clauses from contracts, thus saving hundreds of hours of manual labour.

### What is the CUAD Dataset?

In March 2021, the Atticus Project released the Contract Understanding Atticus Dataset (CUAD), which consists of over 500 contracts, each carefully labelled by legal experts, to identify 41 different types of important clauses, for a total of more than 13,000 annotations. Alongside the dataset, they also published several state-of-the-art Transformer models that have been trained on the dataset. You can find the dataset and the training code at their GitHub repo, and the fine-tuned models can be downloaded from Zenodo.

### What is the BERT for CUAD?

  BERT stands for Bidirectional Encoder Representations from Transformers. Unlike recent language representation models, BERT is designed to pre-train deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task-specific architecture modifications.

  BERT is conceptually simple and empirically powerful. It obtains new state-of-the-art results on eleven natural language processing tasks, including pushing the GLUE score to 80.5% (7.7% point absolute improvement), MultiNLI accuracy to 86.7% (4.6% absolute improvement), SQuAD v1.1 question answering Test F1 to 93.2 (1.5 point absolute improvement) and SQuAD v2.0 Test F1 to 83.1 (5.1 point absolute improvement). 

  This repository contains 3 jupyter notebook. The notebooks contains the steps to download the original repository from the Atticus Project, the steps to download the Bert model and a walk through to install the necessary dependencies. Please run the notebooks in order starting with 1_preparation.jpynb

Notebook 3 contains an implementation of Tesseract OCR. With Tesseract is possible to extract the text from an image to later feed the model with that text.

**Project:** 

https://www.atticusprojectai.org/cuad

**Git Hub of the project:** 

https://github.com/TheAtticusProject/cuad

**CUAD Dataset:** 

https://huggingface.co/datasets/cuad

*Bert models are under Apache License 2.0*

** ** 
**Benetti Mauro 05.2022**

**License: CC BY 4.0** 

###### https://creativecommons.org/licenses/by/4.0/
