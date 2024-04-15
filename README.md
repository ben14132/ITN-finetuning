# ITN-finetuning

## Finetuning
newllamafinetune.ipynb includes the steps taken to finetune a llama 2 7b model to perform ITN tasks. It requires a hugging face account and a connection to a google drive. It also requires the use of a training file in json format. The data in the training file needs to have a specific format which includes an instruction, input and output. The input is the sentence in spoken form while the output is the same sentence in written form. An example of a training file is shown in trainfile.json. After training, reminder to change the PEFT_MODEL to the huggingface path of the new finetuned model to inference it.

## Model Evaluation
After finetuning the model, it needs to be evaluated. A set of test sentences is then input into the model and the output for each sentence is recorded. The WER for each output is then calculated. The code used to do this is shown in evaluation.ipynb. It requires the use of an excel test file with an example test file shown in testingNumberFormat.xlsx. The input column contains the test sentences that will be input into the model. The hypothesis will be the output given by the model. The output column is the correct output. The WER column is the WER for each sentence. Reminder to change the PEFT_MODEL to the huggingface path to the finetuned model.
