# Regressão Linear - Desenvolvimento e Implementação Algoritmo

Este trabalho foi desenvolvido no âmbito da disciplina de Programação da Pós Graduação Data Science e Business Inteligence.

## Visão Geral

O objetivo deste programa é o desenvolvimento e implementação de um algoritmo que faça regressão linear entre variáveis e o output da função.

## Exemplo de Aplicação

Como requisito do trabalho, colocamos aqui um exemplo prático de como podemos usar o modelo de regressão linear.

## Requisitos

Bibliotecas utilizadas:
- numpy: somente para facilitar operações
- matplotlib: para fazer plot da representação gráfica
- sklearn.datasets: para efeitos de geração de conjunto de dados sintéticos para teste e experimentação

# Exemplo de Uso do Algoritmo desenvolvido

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn.datasets import make_regression

## Criar um conjunto de dados gerados artificialmente para efeitos de testagem do modelo
X, y = make_regression(n_samples=300, n_features=1, noise=10, random_state=42)

## Criar e treinar o modelo de regressão linear
model = linear_regression_fit(X,y) 

## Fazer previsões para o conjunto de dados
X_test = np.linspace(X.min(), X.max(), 100).reshape(-1, 1) #cria uma sequência de 100 pontos espaçados de igual maneira entre o valor mínimo e máximo de X, e faz a distribuição destes dados numa matriz
predictions = predict(X_test, model)

## Plotar os dados e as previsões
plt.scatter(X, y, label="Dados de Treino")
plt.plot(X_test, predictions, color='red', label="Previsões")
plt.xlabel("X")
plt.ylabel("y")
plt.title("Regressão Linear")
plt.legend()
plt.show()
```


![Regressão](https://github.com/SarOliveira3/programming/blob/main/regress%C3%A3o_linear.png)https://github.com/SarOliveira3/programming/blob/main/regress%C3%A3o_linear.png)

## Autores
- Raquel Cunha & Sara Oliveira






