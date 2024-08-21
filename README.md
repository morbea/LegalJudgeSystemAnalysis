# Project Overview
This project investigates the relationship with the legal system in Israel, utilizing the [Knesset Corpus](https://huggingface.co/datasets/HaifaCLGroup/KnessetCorpus) dataset. This dataset contains over 32 million sentences from all the plenary and committee protocols held in the Israeli parliament (Knesset) from 1992 to 2022. For this analysis, we focus on data from the Legal Committee, though future analyses may incorporate data from other committees and plenaries.


# Files

## Folder - data_preperation
This directory is responsible for pulling and preparing data from the server.

**knesset_corpus_filtering.ipynb**:  Retrieves data from ElasticSearch and saves it to Google Drive.
**knesset_scroller.ipynb**: Scrolls through Wikipedia pages to gather information on ministers for each government.

## Folder - training and testing


**lable_data_by_openai_api_platform.ipynb**: Labels the data using the OpenAI API.
**fine_tune_hebert_before_pred_final.ipynb**:  Fine-tunes the HeBERT model.
**tag_data_by_Hebrew_Bert_fine_tuned_machine.ipynb**: Tags the Knesset Corpus data using the fine-tuned HeBERT model.

## Statistical_analysis.ipynb
This notebook provides data exploration and statistical analysis of both labeled and unlabeled data, including statistical tests.

## labeled1.xlsx
This fiile contains the labeled dataset used for training the machine learning model in this project. 
