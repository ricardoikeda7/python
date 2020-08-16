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

### Listar as 5 primeiras linhas do dataset
df.head()

### Várias informções do dataset
df.info()

### Informções das colunas numéricas (count, mean, std, min, 25%, 50%, 75%, max)
df.describe()

### Mostrar quantidade de linhas e colunas
df.shape

### Contar e exibir a quantidade de itens na coluna
df['nome da coluna'].value_counts()

### Renomear colunas
df.rename(columns={'Primeiro nome':'nome','numero':'num'},inplace=True)

### Visualizar quantidade de colunas e linhas
df.shape
