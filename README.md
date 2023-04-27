# RoBERTa Finetuned on SQUAD Dataset
RoBERTa-base was finetuned on SQUAD v1 question-answering dataset. Please visit Hugging Face hosted API of the model: https://huggingface.co/sooolee/roberta-base-finetuned-squad-v1 

For BERT-base-cased finetuned on SQUAD v1 question-answering: https://huggingface.co/sooolee/bert-finetuned-squad-v1

## Model Description and Limitations
* The model "extracts" the relevant information from the context to answer a question. 
* At the moment, the model cannot handle a long context. 

## Training Hyperparameters
The following hyperparameters were used during training:

* learning_rate: 2e-05
* gradient_accumulation_steps: 2
* optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
* lr_scheduler_type: linear
* num_epochs: 3

training_loss=0.77257

## Evaluation Results
* f1 on SQUAD = 92.296
* exact_match on SQUAD = 86.045
