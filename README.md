# CSSE416Project - Talor Swift LLM

## Overview
* This repository contains all the Jupyter notebooks and datasets for our project
* The repo comprises three main folders:
  * Llama2 - contains the main fine-tuning notebook along with notebooks used to load the fine-tuned model and generate test responses
  * ResultProcessing - contains notebooks used to analyze feedback from the Google survey
  * dataset - the data used for fine-tuning and testing
  
## Packages
All dependencies are installed during the execution of the notebooks.


## Running the Code
**Make sure to run the notebook in Google Colab with T4**

* ### Running Fine-tuning Notebook
  * You need a Hugging Face account with an access token
  * After creating a Hugging Face account, you need to ask for permission for the Llama2 model
    *   Request access from [Meta](https://ai.meta.com/resources/models-and-libraries/llama-downloads/). **Make sure to use the same email used in Hugging Face account creation**
    *   Request access from [Hugging face](https://huggingface.co/meta-llama/Llama-2-7b-hf). This could take some time for human approval
  * make sure `train.json` is on the same directory level as the notebook
  * The notebook has comments to explain various parts of the code
  * The latest model and various model checkpoint configurations will be saved to the local folder on Google Colab
  * Save at least one fine-tuned model by using the file explorer on Google Colab and drag the desired model into `content > drive > MyDrive`

* ### Running Test Generation Notebook
  * Still, you need a Hugging Face account with access token
  * In the fifth code block, replace the `new_model` string the location where you saved the model config. It should be something like the following:
```
new_model = "/content/drive/MyDrive/{your_model_config_location}"
```

* ### Runing Analysis Notebook
  * make sure `Taylor Swift or AI_.csv.zip` is on the same directory level as the notebook
  
