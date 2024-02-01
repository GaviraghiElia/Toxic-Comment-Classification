# Toxic-Comment-Classification

```
Erba Sandro – 856327
Galli Alice Hoa – 856648 
Gaviraghi Elia - 869493
```

## Folder Structure 

```
┣ 📂 progetto \                                # Root directory
┣ ┣ 📂 dataset\                                # training and test set CSV
┣ ┃ ┣ 📄 train_info_clean.csv                  # training set CSV after cleaning 
┣ ┃ ┣ 📄 train_info_dirty.csv                  # original CSV
┣ ┃ ┣ 📄 val_info.csv                          # test set CSV
┣ ┣ 📂 matlab_script\                 
┣ ┃ ┣ 📄 alex_net_on_validation.m
┣ ┃ ┣ 📄 clean_and_augment_dataset.m
┣ ┃ ┣ 📄 clustering_features.m                 # script for cleaning dirty dataset
┣ ┃ ┣ 📄 from_folder_to_subfolder.m            # obtain foldering dataset from the original dataset
┣ ┃ ┣ 📄 from_subfolder_to_one_folder.m        # the inverse process
┣ ┣ 📂 notebook\                               # colab files
┣ ┃ ┣ 📄 MobileNetV3.ipynb                     # main notebook where we fine-tuning the selected model
┣ ┃ ┣ 📄 Category_Search_foodx251.ipynb        # category search with selected method using our fine-tuned model
┣ ┃ ┣ 📄 Category_Search_foodx251_cheat.ipynb  # a little bit alternative method for category search
┣ ┃ ┣ 📄 Category_Search_imagenet.ipynb        # inital and alternative method with CNN trained on ImageNet
┣ ┣ 📄 Presentazione Visual.pdf
┣ ┣ 📄 Presentazione Visual.pptx
┣ ┣ 📄 README.md                               # it's me!
```

## 🛠 Istruzioni per l'uso
Per eseguire i notebook del progetto, basta caricarli su Google Colab e lanciare l'esecuzione. Assicurati di cambiare i path inseriti nel progetto con i tuoi percorsi personali.

### Dataset
I dataset utilizzati per il progetto sono disponibili per il [download a questo link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
È stato effettuato il merge del test set: assicurati semplicemente di assegnare il CSV con le label alla variabile `y_test` oppure effettua il merge in locale del CSV

### ✅ Valutazione con un test set
Se vuoi testare i nostri modelli solo sul test set, assicurati di eseguire queste porzioni di codice:
1. Preliminary options
2. Dataset
3. Tokenization
Ora puoi eseguire direttamente il codice che trovi nella sezione test set.


## ⚙️ Software and Hardware Requirement
Sono raccomanti i seguenti requisiti software e hardware
 - Assicurati di avere a disposizione i dataset utili per l'esame. 
 - Google Colab (o Kaggle, ma assicurati di adattare il codice) connesso al runtime con una T4 GPU o simili per poter utilizzare in tempi brevi le reti 
 - Se vuoi eseguire il notebook in locale, assicurati di utilizzare un PC con installato Python 3 e di avere a disposizione una GPU NVidia. Puoi controllare il [supporto della tua GPU a questo link](https://www.tensorflow.org/guide/gpu)
