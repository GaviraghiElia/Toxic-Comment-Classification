# Toxic-Comment-Classification

```
Erba Sandro – 856327
Gaviraghi Elia - 869493
```

## Folder Structure 

```
┣ 📂 project\                              # Root directory
┣ ┣ 📂 dataset\                            # folder containing datasets
┣ ┃ ┣ 📄 train.csv                         # CSV of the training set
┣ ┃ ┣ 📄 test_merged.csv                   # modified CSV of the test set
┣ ┃ ┣ 📄 val_info.csv                      # test set CSV
┣ ┣ 📂 Transformers\                 
┣ ┃ ┣ 📄 transformer BERT.ipynb            # Colab notebook for BERT transformers
┣ ┣ ┣ 📂 Best_Model\
┣ ┃ ┃ ┣ 📄 transformer BERT.ipynb          # Colab notebook for BERT transformers
┣ ┣ 📂 RNN\                 
┣ ┃ ┣ 📄 .safetensor, .json, .txt,...      # BERT transformer files
┣ ┣ ┣ 📂 GloVe\                            # folder containing two pretrained embeddings
┣ ┃ ┃ ┣ 📄 glove.840B.300d.txt
┣ ┃ ┃ ┣ 📄 glove.twitter.27B.200d.txt 
┣ ┣ ┣ 📂 Best_Model\                       # Keras models of the best RNNs
┣ ┃ ┃ ┣ 📄 best_RNN_tuned.h5               # best RNN with hyperparameter tuning
┣ ┃ ┃ ┣ 📄 best_RNN_840b_embedded.h5       # best RNN with 840B.300d embedding
┣ ┃ ┃ ┣ 📄 best_RNN_twitter_embedded.h5    # best RNN with Twitter embedding
┣ ┣ ┣ 📂 Tuning_Result\                    # tuning checkpoints for various RNNs tested
┣ ┣ 📂 Report\                 
┣ ┃ ┣ 📄 report.pdf                        # project report in PDF
┣ ┃ ┣ 📄 report.zip                        # LaTeX source code for the report
┣ ┣ 📄 Presentation AML.pdf                # exam presentation PDF
┣ ┣ 📄 Presentation AML.pptx               # exam presentation PowerPoint
┣ ┣ 📄 README.md                           # it's me!
```

## 🛠 Instructions for use
To run the project notebooks, you need to upload them to Google Colab, connect to the T4 GPU runtime and launch execution. Make sure to **change the paths** you have in your project with your own personal paths.

### Dataset
The datasets used for the project are available for [download at this link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
The test set has been merged: you can proceed by modifying a line of code, or by assigning to `y_test' the CSV containing the test set labels, or merge the CSV concerning the test set locally.

### ✅ Test set
If you want to test our models only on the test set, make sure to run these portions of code:
1. Preliminary options
2. Dataset
3. Tokenization
Now you can directly run the code that you find in the test set section.
If you want to upload your own personal test set, please follow the format presented in the kaggle challenge.

## ⚙️ Software and Hardware Requirement
The following software and hardware requirements are recommended
 - Google Colab (or Kaggle, but make sure to adapt the code) connected to the runtime with a T4 GPU or similar to be able to use networks in short time 
 - To run the notebook locally, make sure you are using a PC with Python 3 installed and have a NVidia GPU available. You can check the [support of your GPU at this link](https://www.tensorflow.org/guide/gpu)
