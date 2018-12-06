
* Pacotes utilizados
-numpy
-pandas
-pickle
-timeit
-sklearn
-logging
-pytorch


* Execução do código

O código para executar esse projeto encontra-se em jupyter notebooks. Foram desenvolvidos três notebooks:

**1_Data_Prep.ipynb**: Esse notebook lê a base de dados original do CETENFolha e faz os pré-processamentos necessários nas sentenças. No fim do notebook, uma base pré-processada é salva no arquivo "preprocessed_CETEN_v2.pkl".

**2_Train-LSTM.ipynb**: Esse notebook carrega a base pré-processada e é responsável por definir a arquitetura da rede neural e também por fazer o treinamento da rede. É necessário fazer o download do arquivo glove_s50.zip do Nilc. No fim do notebook, os pesos da rede e alguns dicionários auxiliares são salvos nos arquivos model_96acc_bs1_state_dict.model e model_lstm_dicts.pkl.

**3_Evaluate-LSTM.ipynb**: Esse notebook carrega a rede treinada no notebook anterior juntamente com a base pré-processada e avalia o modelo em toda a base de teste (com 5-fold cross validation).
