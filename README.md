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
## Results
### Discriminator
It doesn't seem to be trained enough.
Adding an MLP layer to DistilBERT or BERT seems to be more efficient than Llama prompt tuning for solving binary classification problems.
### Generator
Sentiment scores
Model1 : 0.495  / Model2 : 0.576  / Model3 : 0.546
Cossim
Model1 : 0.177  / Model2 : 0.298  / Model3 : 0.292
Model2 learned most effectively at learning rate=3e-4 and Epochs=100.
