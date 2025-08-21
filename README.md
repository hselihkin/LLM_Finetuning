# LLM_Finetuning
This project aims to train and evaluate transformer models for English-to-Hindi translation, using the IITB English-Hindi Parallel Corpus as the dataset. The primary goal is to compare different training techniques by fine-tuning a pre-trained model and then assessing its performance against the original, non-fine-tuned version. This comparison is achieved by fine-tuning the model on a subset of the dataset and then using standard machine translation metrics like BLEU, ROUGE, and METEOR to measure the impact of fine-tuning on translation quality.

The project leverages the MarianMT transformer architecture, specifically the pre-trained 
Helsinki-NLP/opus-mt-en-hi model from Hugging Face, implemented in TensorFlow. The methodology involves loading a subset of 100,000 samples from the dataset, preparing the text with an 

AutoTokenizer, and fine-tuning the TFAutoModelForSeq2SeqLM using an Adam optimizer. This process adapts the general-purpose pre-trained model to the specific nuances and characteristics of the English-Hindi dataset, ultimately enhancing its translation accuracy
