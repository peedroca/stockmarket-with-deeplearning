# Mercado de ações com Deep Learning

Neste repositório abordarei algumas técnicas de Machine Learning e Deep Learning para predições no mercado de ações.

![CSNA3](/CSNA3/Análise%20Técnica%20CSNA3.png)

# Performance dos modelos - Classificação com LSTM AutoEncoder e Gradiant Boosting

## Backing Test 2023

Ação|Abertura|Fechamento|Lucro/Perda percentual|Valor Aplicado|Valor Final
:--|:--|:--|:--:|:--|:--
CSNA3.SA|R$13.42|R$19.66|44.65%|R$1000.00|R$1446.55
BBAS3.SA|R$30.70|R$55.39|42.02%|R$1000.00|R$1420.17
VALE3.SA|R$84.08|R$77.20|1.45%|R$1000.00|R$1014.49
PETR4.SA|R$17.76|R$37.24|0.00%|R$1000.00|R$1000.00

## Avaliação das classificações - Dataset Test

Ação|Precisão na Venda|Precisão na Compra|Acurácia
:--|:--:|:--:|:--:
CSNA3.SA|77%|77%|77%
BBAS3.SA|75%|61%|69%
PETR4.SA|60%|78%|65%
VALE3.SA|58%|60%|59%

# Container usado nos tests
Execute o comando abaixo para criar um Container com Tensorflow e Jupyter:
```bash
docker run --name tf -p 8888:8888 jupyter/tensorflow-notebook
```

# Referências

- [A novel deep learning framework: Prediction and analysis of financial time series using CEEMD and LSTM](https://www.sciencedirect.com/science/article/abs/pii/S0957417420304334)
- [A Gentle Introduction to LSTM Autoencoders](https://machinelearningmastery.com/lstm-autoencoders/)