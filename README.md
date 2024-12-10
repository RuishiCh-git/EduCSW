# EduCSW - Building a Mandarin-English Code-Switched Generation Pipeline for Computer Science Learning
This repository presents EduCSW, a novel pipeline for generating synthetic code-mixed datasets, with a specific implementation focusing on Mandarin-English code-switching in computer science education. 

The project offers:
1. A generalizable pipeline architecture for creating code-mixed text datasets
2. A concrete implementation demonstrating the pipeline's effectiveness in generating a computer science education corpus
3. Resources and code for adapting the pipeline to other language pairs and domains

Our proof-of-concept implementation specifically targets Chinese students studying computer science in English-language environments, addressing the need for code-switched educational content that bridges language transitions in technical learning.
The generated datasets are designed to support downstream tasks such as training educational chatbots and developing adaptive learning systems that can adjust their language mixing based on student proficiency levels.

## Dataset Used in This Study: 
*Domain-Specific Dataset -- Computer Science Education Corpus* -- [2imi9/llama2_7B_data_10G](https://huggingface.co/datasets/2imi9/llama2_7B_data_10G)
*Mandarin-English Code-Mixed Dataset -- Transcripts* -- [CAiRE/ASCEND](https://huggingface.co/datasets/CAiRE/ASCEND) and the translated version is here [RuishiCh0314/ASCEND-mixed-to-chinese-translation](https://huggingface.co/datasets/RuishiCh0314/ASCEND-mixed-to-chinese-translation)

## Preparation Stage: 
*EduCSW_Data_Preparation_1.ipynb* -- this notebook documents parallel corpus creation, alignment texts processing, and feature extraction using BERT-NER ([dbmdz/bert-large-cased-finetuned-conll03-english](https://huggingface.co/dbmdz/bert-large-cased-finetuned-conll03-english])).

*EduCSW_Data_Preparation_2 Pre-trained NMT Model* -- This pre-trained NMT model is stored here: [yl31/opus-mt-zh-en-finetuned-cs-instruction](https://huggingface.co/yl31/opus-mt-zh-en-finetuned-cs-instruction)

## Code-Mixed Data Generation: 
*EduCSW_Fine-tune_NMT Model* -- The model is stored here: [yl31/code-mixed-cs-edu-model](https://huggingface.co/yl31/code-mixed-cs-edu-model). 

*EduCSW_Encoder_Decoder_Architecture.ipynb* -- this notebook specifically documents the entire encoder-decoder code-mixed data generation model (along with training, implementation, as well as quick evaluation). The trained weights are saved on hugging face: [RuishiCh0314/EduCSW_model](https://huggingface.co/RuishiCh0314/EduCSW_model).


 
