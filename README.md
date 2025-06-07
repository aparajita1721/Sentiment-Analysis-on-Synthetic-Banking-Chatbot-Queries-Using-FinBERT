# Sentiment-Analysis-on-Synthetic-Banking-Chatbot-Queries-Using-FinBERT
## Model Used
`yiyanghkust/finbert-tone` (used for validation purposes)

## Dataset
Synthetically generated banking chatbot dataset

## Project Description
This project detects whether a customer message is **positive**, **negative**, or **neutral** to better understand their emotional state. It helps identify frustrated or satisfied customers, prioritize chatbot improvements, and guide better response strategies.

It demonstrates skills in **Natural Language Processing (NLP)**, **sentiment analysis**, and **generative modeling**, all of which are essential for improving chatbot helpfulness and the overall banking customer experience.

## Methodology
We used **FinBERT**, a model fine-tuned on financial texts, and evaluated its performance on sentiment analysis.

The model was tested on a synthetically generated dataset to predict sentiment labels of chatbot-style queries. It performs **poorly on this data**, with an overall accuracy of just **41%**. It heavily favors predicting **neutral sentiment** (recall of 88%) but completely fails to identify **positive sentiment** (0% recall and precision). While it captures some negative cases, the precision is low.

This indicates that the model, trained on financial news, **struggles to generalize to chatbot-style conversations**, especially when detecting positive tone.

## Insights
The sentiment distribution plot shows that **FinBERT predicts mostly neutral sentiment** and misses positive sentiments entirely, further highlighting its **poor generalization to conversational banking queries**.
