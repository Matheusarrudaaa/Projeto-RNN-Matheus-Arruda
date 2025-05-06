# Projeto-RNN-Matheus-Arruda

  O projeto consiste na implementação de uma Rede Neural Recorrente para previsão de demanda de um certo produto no tempo, em 1-3 meses anteriores a sua data. Atualmente, na empresa fictícia, já existe um algoritmo de previsão utilizando a média móvel dos valores no intervalo de tempo de interesse.
  O objetivo é obter resultados superiores à média móvel, e realizar uma análise qualitativa dos dados, e verificar quais fatores mais se relacionam aos padrões encontrados.

## Como Executar

É disponibilizado o notebook com o código fonte em Python. É importante se atentar ao import dos datasets, que são dois: tbl_vendas_mensais.csv e tbl_previsao_sop.xlsx.

O caminho desses dois arquivos precisa estar devidamente sinalizado na segunda linha de código, logo na parte inicial da Análise Exploratória dos dados.

## Bibliotecas Utilizadas

foram utilizadas as seguintes bibliotecas:

# Import das libs utilizadas

# Manipulação de dados
import pickle
import pandas as pd
import numpy as np
from datetime import datetime, timedelta
import re
from textwrap import wrap
from statsmodels.tsa.stattools import acf, pacf #!pip install statsmodels
import statsmodels.api as sm
# Gráficos
import matplotlib.pyplot as plt
import seaborn as sns
from plotly.subplots import make_subplots
import plotly.graph_objects as go
import plotly.express as px
import plotly.io as pio
# Modelagem - Série Temporal
from keras.models import Sequential #!pip install keras e !pip install tensorflow
from keras.layers import Dense, Dropout, LSTM
from sklearn.preprocessing import StandardScaler #!pip install sklearn
from keras.callbacks import ModelCheckpoint



