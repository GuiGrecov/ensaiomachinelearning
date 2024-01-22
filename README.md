# Ensaio de Machine Learning
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/17f13472-8405-42b4-8ad9-74f8009b3343)

# Problema de Negócio


## Descrição
A empresa Data Money acredita que a expertise no treinamento e ajuste fino dos algoritmos, feito pelos Cientistas de Dados da empresa, é a principal motivo dos ótimos resultados que as consultorias vem entregando aos seus clientes.


## Objetivo

O objetivo desse projeto será realizar ensaios com algoritmos de Classificação, Regressão e Clusterização, para estudar a mudança do comportamento da performance, a medida que os valores dos principais parâmetros de controle de overfitting e underfitting mudam.

# Planejamento da solução

## Produto final

O produto final será 7 tabelas mostrando a performance dos algoritmos, avaliados usando múltiplas métricas, para 3 conjuntos de dados diferentes: Treinamento, validação e teste.

## Algoritmos ensaiados

###  Classificação

1. Algoritmos: KNN, Decision Tree, Random Forest e Logistic Regression
2. Métricas de performance: Accuracy, Precision, Recall e F1-Score

###  Regressão

1. Algoritmos: Linear Regression, Decision Tree Regressor, Random Forest Regressor, Polinomial Regression, Linear Regression Lasso, Linear Regression Ridge, Linear Regression Elastic Net, Polinomial Regression Lasso, Polinomial Regression Ridge e Polinomial Regression Elastic Net
2. Métricas de performance: R2, MSE, RMSE, MAE e MAPE

###  Clusterização
1. Algoritmos: K-Means e Affinity Propagation
2. Métricas de performance: Silhouette Score

## Ferramentas utilizadas 
1. Python 3.8 e Scikit-learn

# Insights

## 1º Classificação - Modelo baseado em árvores (Randon Forest): 
Durante o ensaio de classificação, os modelos baseados em árvores obtiveram as melhores métricas de performance e mesmo submetendo o algoritmo a dados não vistos no treinamento houve uma pequena diminuição das métricas. Concluindo assim que o algoritmo não teve overfitting.

## 2º Regressão - piores métricas: 

O teste de regressão obtiveram métricas muito inferiores a todos os treinos. Com isso, fica evidente que é necessário criar novas variáveis e fazer uma realização de features, como também, caso seja necessário podemos coletar mais dados e outras variáveis em outras planilhas (banco de dados). 

## 3º Regressão - Decision Tree Regresson (Overfitting)
Durante o ensaio de regressão, o algoritmo Decision Tree Regressor chegou a quase um R² de 1.00 demonstrando que o modelo representava quase em sua totalidade a variação dos dados, mas essa grande representativade foi devido ao algoritmo ter decorado os dados de treinemanto, isso pode ser confirmado quando ele foi submetido a novos dados e que o algoritmo nunca tinha visto, chegando a um R² negativo.

## 4º Clusterização
A métrica média do Silhouette Score foi de 0.22 - 0.25 é considerado  razoável, mas não excelente. É um indicativo de que os clusters têm alguma separação, mas ainda pode haver alguma sobreposição ou confusão entre eles. Em geral, quanto mais próximo o Silhouette Score estiver de +1, melhor é a qualidade da clusterização. Como não temos o contexto da onde veio os dados e para que será utilizado não podemos afirmar se a métrica é boa! Porém o que sabmos é que está baixa do +1 idealmente sugerido pelo algoritmo. 


# Resultados 

## Classificação 

### Treino
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/57af6cf7-c9ee-4507-99e9-f35cef7c453b)

#### Validação
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/0e96a043-d653-4b14-9098-461231332b18)

### Teste
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/5f305b9a-04ac-45a0-b355-9023a0fcceac)

## Regressão

### Treino 
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/5fdecfad-c97b-44eb-9c72-e779b3aeb7d6)

### Validação
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/70667233-fa0a-4e14-8de5-e8b7c8b272a3)

### Teste 
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/21071ede-8771-4ec9-be77-448f6911c915)


## Clusterização
![image](https://github.com/GuiGrecov/ensaiomachinelearning/assets/94385953/ebbd0be4-362d-42f4-8684-b83171c279c3)




