# Projetos Ciência de Dados

---

## Case 1: **Previsão**

O departamento de RH coletou dados dos funcionários e gostaria que você fizesse a previsão de quais são mais propensos para sair do emprego.
- Base de dados: https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset

## Solução
- Foram usadas as bibliotecas Scikit-Learn, TensorFlow, Numpy, Pandas, Matplotlib, Seaborn e Pickle.
- Algoritmos usados para fazer a previsão, Regressão Logística e Florestas Aleatórias com Scikit-Learn e Redes Neurais Artificiais com o TensorFlow.
- Tratamento dos dados foi feito usando os algoritmos do Scikit-Learn, OneHotEncoder e MinMaxScaler. E também, as bibliotecas Pandas e Numpy.

O Jupyter Notebook correspondente a este projeto é o 'rh.ipynb', está todo documentado e com maiores detalhes do case.

---

## Case 2: **Agrupamento**

Você foi contratado por um banco para analisar os dados e dividir os clientes em pelo menos 3 grupos.

- Base de dados: https://www.kaggle.com/arjunbhasin2013/ccdata

## Solução
- Foram usadas as bibliotecas Scikit-Learn, TensorFlow, Matplotlib, Seaborn, Numpy e Pandas.
- Algoritmos usados para fazer o agrupamento, KMeans, usando o Elbow Method para definir o número de clusters.
- Normalização dos dados usando o StandarScaler do Scikit-Learn.
- Redução da dimensionalidade usando Principal Component Analisys (PCA) e AutoEncoders.
- O que é PCA? É um algoritmo de aprendizagem não supervisionada que aplica redução de dimensionalidade, porém, tenta manter as informações originais com as mesmas características. Encontra um novo conjunto de características que são chamados de componentes, os componentes são criados por meio das características **não** correlacionais. Você vai encontrar um artigo **muito bom** sobre PCA aqui: https://towardsdatascience.com/principal-component-analysis-pca-with-scikit-learn-1e84a0c731b0

- E Autoencoders, o que são? Autoencoders (AE) são redes neurais que visam copiar suas entradas para suas saídas. Eles trabalham compactando a entrada em uma representação de espaço latente e, em seguida, reconstruindo a saída dessa representação. Esse tipo de rede é composto de duas partes:

  - Codificador (Encoder): é a parte da rede que compacta a entrada em uma representação de espaço latente (codificando a entrada). Pode ser representado por uma função de codificação h = f (x).

  - Decodificador (Decoder): Esta parte tem como objetivo reconstruir a entrada da representação do espaço latente. Pode ser representado por uma função de decodificação r = g (h).

  - Funcionam se existir correlação entre os dados de entrada (resultados ruins se os dados de entrada são todos independentes).
  - Uma maneira de obter recursos úteis do Autoencoder é restringir h a ter dimensões menores que x; nesse caso, o Autoencoder é chamado de incompleto. Ao treinar uma representação incompleta, forçamos o Autoencoder a aprender os recursos mais importantes dos dados de treinamento. Leia mais sobre essa técnica: https://www.deeplearningbook.com.br/introducao-aos-autoencoders/

- Para visualização gráfica dos clusters foram usadas as bibliotecas Seaborn e Matplotlib.

O Jupyter Notebook correspondente a este projeto é o 'marketing.ipynb', está todo documentado e com maiores detalhes do case.

---

## Case 3: **Previsão Vendas**

Neste projeto, você foi contratado como um cientista de dados de uma rede de lojas físicas, tendo os dados de 1.115 lojas. Seu objetivo é prever vendas futuras.

- Base de dados: https://www.kaggle.com/c/rossmann-store-sales/data

## Solução
- Foram usadas as bibliotecas Matplotlib, Seaborn, Pandas, Numpy, Datetime e Prophet
- O tratamento dos dados foi feito usando as bibliotecas Pandas, Numpy e Datetime. A visualização dos dados foi realizada com o auxílio das bibliotecas Matplotlib e Seaborn.
- Já as previsões foram feitas com a biblioteca do Facebook, fbprophet (séries temporais). Prophet é um framework criado pelo próprio time de cientistas de dados do Facebook, com o intuito de realizar previsões com séries temporais.
  - O que são séries temporais?
      Nada mais que uma coleção de observações feitas sequencialmente ao longo do tempo. No nosso caso, vendas em período de tempo. Detalhe importante sobre time series (do inglês), a ordem dos dados é fundamental.
 
 Mais informações sobre séries temporais: https://www.inf.ufsc.br/~marcelo.menezes.reis/Cap4.pdf
 
 O Jupyter Notebook correspondente a este projeto é o 'previsao_vendas.ipynb', está todo documentado e com maiores detalhes do case.
