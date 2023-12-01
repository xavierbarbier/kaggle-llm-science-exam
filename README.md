# kaggle-llm-science-exam

## Introduction
This is a spin off from the kaggle-llm-science-exam competition (https://www.kaggle.com/competitions/kaggle-llm-science-exam).
The ideas are :
* multiple-choice question answering (MCQA) task
* use community datasets as training set (more info below)
* use competition training dataset as test set
* compare 2 models (DeBERTa and DistilBERT ) using the competition metric (MAP@3 - www.kaggle.com/competitions/kaggle-llm-science-exam/overview/evaluation)
* use Hugging Face transformers library with Parameter-Efficient Fine-Tuning (PEFT) and LoRa (Low-Rank Adaptation) for training
* push model to Hugging Face hub ad the en of training

NOTEBOOK => https://github.com/xavierbarbier/kaggle-llm-science-exam/blob/main/sci_mutliplechoice.ipynb

## Results
* both model don't reach the setted max epochs (10)
* DeBERTa outperform DistilBERT
* best performance is 0.750833 (still far from competition winners ! - https://www.kaggle.com/competitions/kaggle-llm-science-exam/leaderboard)

* ![image](https://github.com/xavierbarbier/kaggle-llm-science-exam/assets/51788432/97afbb77-2002-4342-bfd7-8cdaf0d96caf)

## Community datasets
* 6000_wiki_en_sci_questions.csv from RADEK OSMULSKI - https://www.kaggle.com/datasets/radek1/sci-or-not-sci-hypthesis-testing-pack
* stem_1k_full_v1.csv from LEONID KULYK - https://www.kaggle.com/datasets/leonidkulyk/wikipedia-stem-1k
* extra_train_set.csv from RADEK OSMULSKI - https://www.kaggle.com/datasets/radek1/additional-train-data-for-llm-science-exam
