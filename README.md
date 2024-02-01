# Toxic-Comment-Classification

```
Erba Sandro – 856327
Galli Alice Hoa – 856648 
Gaviraghi Elia - 869493
```

## Folder Structure 

```
┣ 📂 progetto \                            # Root directory
┣ ┣ 📂 dataset\                            # folder contenenti i dataset
┣ ┃ ┣ 📄 train.csv                         # CSV del training set
┣ ┃ ┣ 📄 test_merged.csv                   # CSV modificato del test set
┣ ┃ ┣ 📄 val_info.csv                      # test set CSV
┣ ┣ 📂 Transformers\                 
┣ ┃ ┣ 📄 transformers.ipynb                # colab notebook della RNN
┣ ┣ 📂 RNN\                 
┣ ┃ ┣ 📄 RNN.ipynb                         # colab notebook del transformers
┣ ┣ ┣ 📂 GloVe\                            # folder contenente due embedding preallenati
┣ ┃ ┃ ┣ 📄 glove.840B.300d.txt
┣ ┃ ┃ ┣ 📄 glove.twitter.27B.200d.txt 
┣ ┣ ┣ 📂 Best_Model\                       # modelli keras delle migliori RNN
┣ ┃ ┃ ┣ 📄 best_RNN_tuned.h5               # miglior RNN con tuning iperparametri
┣ ┃ ┃ ┣ 📄 best_RNN_840b_embedded.h5       # miglior RNN con embedding 840B.300d
┣ ┃ ┃ ┣ 📄 best_RNN_twitter_embedded.h5    # miglior RNN ottenuta con embedding Twitter
┣ ┣ ┣ 📂 Tuning_Result\                    # checkpoint di varie RNNs sperimentate
┣ ┣ 📂 Report\                 
┣ ┃ ┣ 📄 report.pdf                        # PDF report progetto
┣ ┃ ┣ 📄 report.zip                             # codice latex del report
┣ ┣ 📄 Presentazione AML.pdf
┣ ┣ 📄 Presentazione AML.pptx
┣ ┣ 📄 README.md                          # it's me!
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
