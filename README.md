# Rossman Sales Prediction

## Este projeto visa prever numero de vendas de uma rede de farmácias.

#### This project was made by Rômulo Moura.

# 1. Business Problem.
O projeto visa resolver um problema fictício de uma empresa que precisa saber onde(quais lojas) e como  aplicar o budget anual.
Com os dados do Rossman (https://www.kaggle.com/c/rossmann-store-sales) uma rede de farmácias. Após 10 passos do CRISP-DS conseguimos trazer resultados a cerca da previsão de vendas de cada loja em R$, assim o CEO consegue tomar melhores decisões de como irá dividir o budget da empresa.

# 2. Business Assumptions.

# 3. Solution Strategy

My strategy to solve this challenge was:

**Step 01. Data Description:** Descrever estatísticamente os dados dos clientes para tentar entender a forma dos dados.

**Step 02. Feature Engineering:** Criar novas features com base nas já existentes, a fim de melhorar o ranqueamento.

**Step 03. Data Filtering:** Filtrar dados indesejados, sujos, faltantes, que não agregam ao objetivo.

**Step 04. Exploratory Data Analysis:** Encontrar analisando os dados peculiaridades a cerca dos clientes, na finalidade de entender melhor os clientes e melhorar o resultado.

**Step 05. Data Preparation:** Preparar os dados convertendo a formas mais adequadas que os algoritmos de machine learning possam trabalhar.

**Step 06. Feature Selection:** Selecionar as melhores features, aquelas que irão agregar ao resultado esperado, diminuindo a dimensionalidade.

**Step 07. Machine Learning Modelling:** Criação e treinamento dos modelos que farão o ranqueamento dos clientes.

**Step 08. Hyperparameter Fine Tunning:** Após encontrar o melhor modelo, ajustar os parâmetros para melhorar um pouco a capacidade de ranqueamento do algoritmo.

**Step 09. Convert Model Performance to Business Values:** Analisar como os resultados obtidos impactam o negócio da empresa.

**Step 10. Deploy Modelo to Production:** Tornar o modelo público, online, para ser utilizado pela empresa.

# 4. Top 3 Data Insights *Devido se tratar do primeiro ciclo de criação do projeto esta etapa foi adiada.*

**Hypothesis 01:**

**True/False.**

**Hypothesis 02:**

**True/False.**

**Hypothesis 03:**

**True/False.**

# 5. Machine Learning Model Applied
 - Foram criados e comparados 4 modelos de machine learning:
    - K-Nearest Neighbor Classifier
    - Logistic Regression
    - XGBoost Classifier
    - Random Forest Classifier

# 6. Machine Learning Model Performance

|            Model	            |        MAE          |     MAPE          |       RMSE 	       |
| ------------------------------|---------------------|-------------------|------------------- |
|   Random Forest		            |  837.68 +/- 218.12  |	0.12 +/- 0.02	    |	1256.33 +/- 318.28 |
|	  XGBoost Regressor           |	1074.84 +/- 199.67  |	0.15 +/- 0.02     |	1540.63 +/- 278.07 |	
|	  Linear Regression           |	2081.73 +/- 295.63  |	0.3 +/- 0.02      |	2952.52 +/- 468.37 |
|	  Lasso	                      | 2116.38 +/- 341.5   |	0.29 +/- 0.01	    |	3057.75 +/- 504.26 |	

- Random Forest conseguiu os melhores valores de MAE e RMSE, porém é um modelo muito pesado, então foi selecionado o XGBoost para presseguir no projeto.

Após o hyperparameter fine tuning no XGBoost a performance alcançada foi:

| Model Name	      |     MAE	    |    MAPE	  |    RMSE    |
| XGBoost Regressor	| 666.505452	| 0.096956	| 978.003413 |

# 7. Business Results

# 8. Conclusions

# 9. Lessons Learned

# 10. Next Steps to Improve

# LICENSE

# All Rights Reserved - Comunidade DS 2021
