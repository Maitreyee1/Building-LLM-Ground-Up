# Building-LLMs-from-Ground-Up
This repository is created as part of Sebastian Raschka's coding workshop - Building LLMs from Ground Up. The source code in this repository builds GPT2 based LLM from scratch, and also involves pretraining and instruction finetuning the LLms. The repository also contains code to use existing LLM models like OpenAI GPT, Microsoft Phi, Meta LLama, Mistral etc. using LightingAI wrapper. 
The following are some signficant modules and their functionality: 

02_data contains Dataset preparation code for LLM training. 
The data used for this project is the The Verdict- By Edith Wharton. The folder contains the_verdict.txt text file for the same. 
The code contains modules to break down the text into tokens (tokenization), create a vocabulary and convert tokens into numbers that the LLM model can understand. (creating token embeddings).

03_LLM_Architecture contains Jupyter notebook and code for LLM Architectures and building  a LLM. 
It briefs on the Transformer block, LayerNorm, Feed Forward layers and also shows differences between architectures of various LLMs.
The LLM model built from scratch in this module is present in the supplementary.py file and is based on the OpenAI GPT 2 model. 

04_LLM_Pretraining contains Jupyter Notebook and  code about pretraining the LLM model and tracking the loss on the training data and validation data.

05_LLM_Weightloading contains Jupyter notebook explaining the method to add weights to the pretrained model. 
The custom built GPT2 model model is assigned weights and congfigurations based on other existing OpenAI GPT models. 
The folder also contains read-to-use alternatives to building the LLMs model from scratch. LitGPT wrapper provide other LLM models like Microsoft Phi2, OpenLLMA-2 etc. 

06_LLM_Finetuning contains Jupyter Notebook that explains instruction finetuning for LLMs and compares output of the base model and finetuned model.
It also demonstrates usage of low rank adapton technique- (LoRA) for Instruction finetuning. 
The Jupyter Notebook also contains Model Evaluation based on benchmark tests like MMLU, LM Evaluation Harness, AlpacaEval, etc. 

