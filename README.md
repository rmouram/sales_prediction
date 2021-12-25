# sales_prediction

🏗️ ESTE É UM PROJETO EM CONSTRUÇÃO 🏗️ Projeto de Regressão

<p> [X] Obtenção dos dados </p>
<p> [X] Feature Engineering </p>
<p> [X] Filtragem de variáveis </p>
<p> [X] Análise Exploratória </p>
<p> [X] Data Preparation </p>
<p> [X] Feature selection </p>
<p> [X] Machine Learning Moddeling </p>
<p> [X] Hyperparameter Fine Tuning </p>
<p> [X] Tradução e interpretação do erro </p>
<p> [ ] Deploy do modelo em produção </p>
<p> [ ] Criação do bot no telegram </p>

## Sobre o projeto
  <p> Este é um projeto de portifólio com a finalidade de demonstrar e aprender habilidades e técnicas referentes a ciência de dados. </p>
  <p> O projeto visa resolver um problema fictício de uma empresa que precisa saber onde(quais lojas) e como  aplicar o budget anual.
  Com os dados do Rossman (https://www.kaggle.com/c/rossmann-store-sales) uma rede de farmácias. Após 10 passos do CRISP-DS conseguimos trazer resultados a cerca da previsão de vendas de cada loja em R$, assim o CEO consegue tomar melhores decisões de como irá dividir o budget da empresa.</p>

## Tecnologias
 - Python
 - Sklearn
 - Xgboost
 - Heroku
 - API Telegram
 
## Como instalar
 1. Crie um ambiente virtual para separar as dependências que serão instaladas.
 2. Faça o clone para o diretório desejado.
 3. Em um terminal e com o ambiente virtual ativado faça: pip install requirements.txt.
 4. Em um terminal digite: mkdir model, isso criará uma pasta para o modelo ser salvo.
 5. Digite jupyter-notebook no terminal.
 6. Ao entrar no arquivo v1.0_store_sales_prediction.ipynb vá em Cell e clique em Run All na aba superior do jupyter.
 7. Após isso poderá demorar horas para concluir devido aos treinamentos de ML e o fine tuning.

## Como testar o modelo offline (Versao online com Heroku ainda nao disponível)
 1. É nessário entrar na pasta api e modificar o arquivo handler.py:
  1.1 Troque o caminho na variável 'path' pelo caminho do seu computador até a pasta sales_prediction.
 2. Então em um terminal digite: python handler.py para iniciar o servidor.
 3. Vá na seção 10.3 API Tester clique no codigo e aprte ctrl + Enter para rodar o codigo.
 4. Caso queira mudar as lojas observadas basta alterar a variável 'list_stores'.
 5. Caso queira verificar as previsões de uma loja específica por dia, na célula abaixo basta alterar a variável 'store' com o 
    valor da loja desejado e rodar com ctrl + Enter. Será mostrado um dataframe, a previsão está em uma coluna 'prediction' ao fim do dataframe.

## Estado do projeto
<p> Estou tendo problemas com o Heroku por isso ainda não é possível testar o projeto sem precisar fazer um clone e gerar o modelo manualmente.</p>
<p> Em breve quando solucionar os problemas também haverá um bot no telegram para facilitar o acesso.</p>

## Autor
<p>https://github.com/rmouram</p>
<p>Rômulo Ferreira</p>
<p>ferreira.moura.maia@gmail.com</p>
## Licença


