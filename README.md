# kaggle-llm-science-exam

## Introduction
This is a spin off from the kaggle-llm-science-exam competition (https://www.kaggle.com/competitions/kaggle-llm-science-exam).
The idea is :
* use community datasets as training set
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

