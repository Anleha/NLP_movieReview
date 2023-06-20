# Movie Review Generation with fine-tuning LLM
Implemetation of the final project: Movie Review Generation with fine-tuning LLM
# Executing the Code
All codes are written and run on google colab.
## Make data file
Run data.ipynb to create data file used for training the LM. The original data is downloaded from kaggle (Link is provided in data.ipynb)
## Train the LM
Run train_generator_final.ipynb to download the pretrained model and finetune it. The output is the 3 finetuned model coressponding to 3 prompt styles.
Run train_discriminator.ipynb to train the discriminator model
## Evaluation
Run eval_and_make_example.ipynb to load the finetuned model for evaluation of each finetuned model.
