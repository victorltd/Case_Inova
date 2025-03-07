# Customer Churn Prediction

## Descrição do Projeto
Este projeto tem como objetivo prever o **Churn de Clientes** (clientes que deixam o banco) com base em dados históricos. Utilizamos técnicas de **análise exploratória de dados (EDA)** e **machine learning** para identificar padrões e desenvolver um modelo preditivo.

O dataset contém informações como:
- **Dados Demográficos**: Idade, Gênero, Localização.
- **Dados Financeiros**: Saldo, Salário Estimado, Pontuação de Crédito.
- **Interações com o Banco**: Número de Produtos, Posse de Cartão de Crédito, Reclamações.

## Objetivo
Desenvolver um modelo de machine learning para prever quais clientes têm maior probabilidade de deixar o banco (Churn), permitindo que a empresa tome ações preventivas para retenção.

## Dados
O dataset utilizado neste projeto é o **Customer Churn Records**, que contém informações sobre clientes de um banco. As principais variáveis incluem:
- **Variáveis Numéricas**: `CreditScore`, `Age`, `Balance`, `EstimatedSalary`, `NumOfProducts`, `Point Earned`.
- **Variáveis Categóricas**: `Geography`, `Gender`, `HasCrCard`, `IsActiveMember`, `Complain`, `Card Type`.
- **Variável Alvo**: `Exited` (Churn).

O dataset está disponível em [Kaggle](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn) ou no arquivo `Customer-Churn-Records.csv` deste repositório.

## Metodologia
1. **Análise Exploratória de Dados (EDA)**:
   - Verificação de valores nulos e tipos de dados.
   - Análise de distribuições e correlações.
   - Identificação de desbalanceamento nas variáveis `Exited` e `Complain`.

2. **Pré-processamento**:
   - Remoção de colunas irrelevantes (`RowNumber`, `CustomerId`, `Surname`).
   - Tratamento de outliers com Winsorization.
   - Codificação de variáveis categóricas (One-Hot Encoding).

3. **Modelagem**:
   - Seleção de features com Random Forest.


4. **Resultados**:
   - As variáveis mais importantes para prever Churn foram `Age`, `Balance`, `NumOfProducts` e `Point Earned`.
  
