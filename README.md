# Construção de ETL em Website de loja de roupa - WebScraping
<span aling="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/ETL_logo.png" width="500px"/>

</span>

Extração - transformação - carregamento (ETL):
  
  - Tal processo é uma combinação de dados de diversas fontes, passando pela etapa de limpeza e organização desses dados brutos, sendo prepadados para o armazenamento, análise e modelagem com algoritmos de Machine Learning.

## 1. Problema de Negócio

A empresa Star Jeans!

Eduardo e Marcelo são dois brasileiros, amigos e sócios de empreendimento. Depois de vários negócio bem sucedidos, eles estão planejando entrar no mercado de moda dos USA como um modelo de negócio do tipo E-commerce.

A idéia inicial é entrar no mercado com apenas um produto e para um público específico, no caso o produto seria calças Jenas para o público masculino. O objetivo é manter o custo de operação baixo e escalar a medida que forem conseguindo clientes. Porém, mesmo com o produto de entrada e a audiência definidos, os dois sócios não tem experiência nesse mercado de moda e portanto não sabem definir coisas básicas como preço, o tipo de calça e o material para a fabricação de cada peça. Assim, os dois sócios contrataram uma consultoria de Ciência de Dados para responder as seguintes perguntas:

1. Qual o melhor preço de venda para as calças?

2. Quantos tipos de calças e suas cores para o produto inicial?

3. Quais as matérias-prima necessárias para confeccionar as calças?

As principais concorrentes da empresa Start Jeans são as americadas H&M e Macys.

## 2. Resolução do Problema de Negócio

### 2.1 Método CRISP-DS de Desenvolvimento

![image1](https://user-images.githubusercontent.com/80589529/210022497-47160142-63c9-4e24-8828-ecd678f71dfa.png)

### Para o Entendimento de Negócio foi utilizado os seguintes critérios:

1. Saída: (Produto Final)

    - Mediana dos preços dos concorrentes, através de tabelas ou gráficos.
  
2. Processo (Passo a Passo) :

    - Coletando os dados através da biblioteca Beautiful soup do Python.
  
    - Com o Pandas, criando um dataframe as principais informações:
  
    id | product_name | product_type | product_color | composition | product_price
    ---- | ------ | ----- | ----- | ----- | ------
  
    - Armazenamento em Banco de Dados (SQLite3)

3. Fonte de dados:

  - Site da H&M: https://www2.hm.com/en_us/men/products/jeans.html
  
### 2.2 Planejamento da ETL - Arquitetura 

Nesse primeiro momento do Ciclo de CRISP é feito a orquestração de 04 Jobs para a produção desse ETL.

- JOB 01 - Coleta de dados na vitrine de calças jeans masculina por meio da biblioteca BS4.
- JOB 02 - Coleta de dados dos detalhes de cada produto e paginação por meio da biblioteca BS4.
- JOB 03 - Limpeza de dados utilizando Pandas.
- JOB 04 - Armazenamento dos dados no Banco de Dados, SQLite3.

![jobs](https://user-images.githubusercontent.com/80589529/210063195-2d675bcd-609c-48c3-a940-8ec55dd57957.png)
 
## Ferramentas:
1. Python 3, Pandas e Beautiful Soup.
2. SQL.
3. GIT e GitHub.
4. Jupyter Notebook ( Analise e prototipagens ) e Visual Studio Code.

## 3. Conclusão.

Finalizado o primeiro ciclo de CRISP proposto, foi criado um ETL que conseguiu extrair os dados do Website da H&M, concorrente da empresa ficticia Star Jeans, com o objetivo de se ter um parametro de modelo de negócio desse produto.

## 4. Próximos Passos.

Para próximas etapas do Projeto, atualização semanal dos dados do concorrente através do gereciador de jobs Apache Airflow, automatizando o processo de ETL. 

## CONTATO

[![linkedin](https://user-images.githubusercontent.com/80589529/210065487-b2bcf8e5-3cc6-43c7-a421-5b095f5f19d2.svg)](https://www.linkedin.com/in/carolcostaf/)
[![gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](folignocaroline@gmail.com)
