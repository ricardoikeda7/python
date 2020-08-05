# python for data analysis
### Importação de bibliotecas (libraries)
import numpy as np 
import pandas as pd
%matplotlib inline
from matplotlib import pyplot as plt 

### Importar o dataset usando wget
!wget -O planilha.csv https://endweb.com.br/labs/planilha.csv

### Importar dataset quando estiver localmente no computador
df=pd.read_csv("data.csv", index_col=1, encoding="latin-1")

### Renomear colunas
df.rename(columns={'Primeiro nome':'nome','numero':'num'},inplace=True)
### Visualizar quantidade de colunas e linhas
df.shape
