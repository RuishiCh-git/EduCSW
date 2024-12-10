# EduCSW
This git aims to propose a pipeline for generating synthetic code-mixed datasets

## Preparation Stage: 
*EduCSW_Data_Preparation_1.ipynb* -- this notebook documents parallel corpus creation, alignment texts processing, and feature extraction using BERT-NER.

*EduCSW_Data_Preparation_2 Pre-trained NMT Model* -- This pre-trained NMT model is stored here: [yl31/opus-mt-zh-en-finetuned-cs-instruction](https://huggingface.co/yl31/opus-mt-zh-en-finetuned-cs-instruction)

## Code-Mixed Data Generation: 
*EduCSW_Fine-tune_NMT Model* -- The model is stored here: [yl31/code-mixed-cs-edu-model](https://huggingface.co/yl31/code-mixed-cs-edu-model). 

*EduCSW_Encoder_Decoder_Architecture.ipynb* -- this notebook specifically documents the entire encoder-decoder code-mixed data generation model (along with training, implementation, as well as quick evaluation). The trained weights are saved on hugging face: [RuishiCh0314/EduCSW_model](https://huggingface.co/RuishiCh0314/EduCSW_model).


 
