# Coleta de Dados em Website de loja de roupa - WebScraping

## Problema de Negócio

A empresa Star Jeans!

Eduardo e Marcelo são dois brasileiros, amigos e sócios de empreendimento. Depois de vários negócio bem sucedidos, eles estão planejando entrar no mercado de moda dos USA como um modelo de negócio do tipo E-commerce.

A idéia inicial é entrar no mercado com apenas um produto e para um público específico, no caso o produto seria calças Jenas para o público masculino. O objetivo é manter o custo de operação baixo e escalar a medida que forem conseguindo clientes. Porém, mesmo com o produto de entrada e a audiência definidos, os dois sócios não tem experiência nesse mercado de moda e portanto não sabem definir coisas básicas como preço, o tipo de calça e o material para a fabricação de cada peça. Assim, os dois sócios contrataram uma consultoria de Ciência de Dados para responder as seguintes perguntas:

1. Qual o melhor preço de venda para as calças?

2. Quantos tipos de calças e suas cores para o produto inicial?

3. Quais as matérias-prima necessárias para confeccionar as calças?

As principais concorrentes da empresa Start Jeans são as americadas H&M e Macys.

## Método CRISP-DS de Desenvolvimento

<img src="https://media-exp1.licdn.com/dms/image/C4E12AQERUhx3Vbo4Mg/article-cover_image-shrink_720_1280/0/1579703817380?e=1669248000&v=beta&t=GHe0XhVAfK4VhX-hEeY5CFusDjV3cRz6yDDhesdeP2o" width="500" />

### Para o Entendimento de Negócio foi utilizado os seguintes critérios:

1. Saída: (Produto Final)

  - Mediana dos preços dos concorrentes, através de tabelas ou gráficos.
  
2. Processo (Passo a Passo) :

  - Coletando os dados através da biblioteca Beautiful soup do Python.
  
  - Com o Pandas, criando um dataframe as principais informações:
  
    id | product_name | product_type | product_color | composition | product_price
  
  - Armazenamento em Banco de Dados (SQLite3)

3. Fonte de dados:

  - Site da H&M: https://www2.hm.com/en_us/men/products/jeans.html
 
### Ferramentas:
1. Python 3
2. Bibliotecas de Webscrapping ( BS4)
3. Visual Studio Code
4. Jupyter Notebook ( Analise e prototipagens )
