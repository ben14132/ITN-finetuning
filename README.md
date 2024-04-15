# ITN-finetuning

## Finetuning
newllamafinetune.ipynb includes the steps taken to finetune a llama 2 7b model to perform ITN tasks. It requires the use of a training file in json format. The data in the training file needs to have a specific format which includes an instruction, input and output. The input is the sentence in spoken form while the output is the same sentence in written form. An example of a training file is shown in trainfile.json
