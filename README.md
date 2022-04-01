![Sales-Forecast-2](https://user-images.githubusercontent.com/28973566/161333971-682a7ee6-2f03-4d9b-97d2-1a8b9f7235f0.jpeg)

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

# 4. Top 3 Data Insights:

**Hypothesis 01:**
Lojas deveriam vender mais ao longo dos anos.
**False.**

![image](https://user-images.githubusercontent.com/28973566/161334401-55b56a07-b0c2-40b0-9bcd-f94a80f280a0.png)

**Hypothesis 02:**
Lojas com competidores próximos deveriam vender menos.
**False.**

![image](https://user-images.githubusercontent.com/28973566/161334588-1c7b5ace-2f39-43de-810b-a81519bfb94e.png)

**Hypothesis 03:**
Lojas deveriam vender mais durante o feriado de natal.
**False.**

![image](https://user-images.githubusercontent.com/28973566/161334697-23e12626-4b3e-4d1a-a849-2a413159039b.png)

# 5. Machine Learning Model Applied
 - Foram criados e comparados 4 modelos de machine learning:
    - Lasso	
    - Linear Regression
    - XGBoost Regressor
    - Random Forest 

# 6. Machine Learning Model Performance

|            Model	            |        MAE          |     MAPE          |       RMSE 	       |
| ------------------------------|---------------------|-------------------|------------------- |
|   Random Forest		            |  837.68 +/- 218.12  |	0.12 +/- 0.02	    |	1256.33 +/- 318.28 |
|	  XGBoost Regressor           |	1074.84 +/- 199.67  |	0.15 +/- 0.02     |	1540.63 +/- 278.07 |	
|	  Linear Regression           |	2081.73 +/- 295.63  |	0.3 +/- 0.02      |	2952.52 +/- 468.37 |
|	  Lasso	                      | 2116.38 +/- 341.5   |	0.29 +/- 0.01	    |	3057.75 +/- 504.26 |	

- Random Forest conseguiu os melhores valores de MAE e RMSE, porém é um modelo muito pesado, então foi selecionado o XGBoost para presseguir no projeto.

Após o hyperparameter fine tuning no XGBoost a performance alcançada foi:

|       Model       |     MAE	   |   MAPE	  |    RMSE    |
|-------------------|------------|----------|----------- |
| XGBoost Regressor	| 666.505452	| 0.096956	| 978.003413 |

# 7. Business Results
Com as previsões de vendas em mãos, foi calculado os ganhos da empresa no pior e melhor cenário.

|     Scenario	  |      Values      |
|----------------|------------------|
| predictions	   | R$274,200,960.00 |
| worst_scenario	| R$273,453,773.10 |
| best_scenario	 | R$274,948,139.99 |

O modelo retorna dado um id de loja, o valor de vendas que a loja terá nas 6 semanas seguintes, desta forma:
"Store number 21 will sell R$222,100.29 in the next 6 weeks"

# 8. Conclusions
O modelo de machine learning conseguiu de forma satisfatória prever vendas com baixos erros.

# 9. Lessons Learned
Este é meu primeiro projeto de data science completo, logo todo conhecimento aplicado aqui foi aprendido neste projeto.

# 10. Next Steps to Improve
- Testar mais modelos de ml.
- Checar desbalanceamento
- Testar PCA.
- Criar mais features

# 11. Deploy

Foi criado um bot no telegram que dado uma entrada de numero de loja, o bot por meio de uma API acessa o heroku onde o modelo está publicado e retorna o valor em vendas daquela loja.

![ds](https://user-images.githubusercontent.com/28973566/161333686-8a239e5c-862a-4ede-8401-d8a5e9707192.png)

# LICENSE

# All Rights Reserved - Comunidade DS 2021
