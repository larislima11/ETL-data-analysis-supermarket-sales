# Supermarket Customer Analysis

Este projeto é uma análise do comportamento de compra dos clientes de um grande supermercado. O objetivo é entender padrões de venda por hora, categorias de produtos mais vendidos, e as características demográficas dos clientes.
Utilizando técnicas de processamento de dados e visualização, esta análise pode ajudar o supermercado a melhorar sua estratégia de marketing e otimizar as operações.

# Objetivo

- Analisar o comportamento de compra dos clientes de um supermercado com base em dados de vendas.
- Entender quais produtos são mais vendidos e identificar padrões de compra ao longo do dia.
- Explorar dados demográficos dos clientes, como idade, gênero e localização, para insights sobre o perfil de compra.

# Tarefas Realizadas

1. Geração de Dados Simulados:

- Criamos três conjuntos de dados simulados, representados em arquivos CSV:
- Vendas: Detalhes sobre cada venda, como produto comprado, valor da compra, hora e cliente.
- Clientes: Informações demográficas dos clientes, como idade, gênero e localização.
- Produtos: Detalhes dos produtos, incluindo categoria e preço.

2. Processamento de Dados (ETL):

- Extração: Extraímos os dados simulados de arquivos CSV.
- Transformação: Realizamos a limpeza dos dados e calculamos métricas importantes, como ticket médio por cliente e quantidade média de itens por compra.
- Carga: Estruturamos os dados em um formato adequado para análise, criando tabelas de fatos e dimensões.

3. Análise e Visualização:

- Volume de Vendas por Hora: Um gráfico de linhas mostrando como as vendas variam ao longo do dia.
- Quantidade de Produtos Vendidos por Categoria: Um gráfico de barras comparando as categorias de produtos mais vendidos.
- Perfil Demográfico dos Clientes: Um gráfico de pizza exibindo a proporção de clientes por faixa etária.

 # Organização dos Dados

clientes.csv: Contém dados demográficos dos clientes.

id_cliente: Identificador único de cada cliente.
idade: Idade do cliente.
gênero: Gênero do cliente (masculino, feminino).
localizacao: Cidade onde o cliente reside.
vendas.csv: Contém informações sobre as vendas realizadas.

id_venda: Identificador único da venda.
id_produto: Produto comprado.
valor: Valor da venda.
hora_compra: Hora do dia em que a venda foi realizada.
id_cliente: Cliente que realizou a compra.
produtos.csv: Contém informações sobre os produtos vendidos.

id_produto: Identificador único do produto.
categoria: Categoria do produto (alimentos, bebidas, etc.).
preco: Preço do produto.

# Visualizações

As visualizações disponíveis no notebook ajudam a entender o comportamento de compra e o perfil dos clientes:

1. Gráfico de Linhas - Volume de Vendas por Hora do Dia:
Este gráfico mostra como o volume de vendas varia ao longo do dia.

2. Gráfico de Barras - Quantidade de Produtos Vendidos por Categoria:
Compara a quantidade de produtos vendidos para cada categoria (alimentos, bebidas, eletrônicos, etc.).

3. Gráfico de Pizza - Proporção de Clientes por Faixa Etária:
Exibe a proporção de clientes em cada faixa etária, mostrando o perfil demográfico dos consumidores.

# Futuras Melhorias
Integração com Firebase: Adicionar a persistência dos dados usando um banco de dados real, como Firebase.
Análise Preditiva: Usar machine learning para prever o comportamento futuro dos clientes.
Análise Geoespacial: Incluir mapas para analisar a localização dos clientes e identificar regiões com maior volume de vendas.

# Contribuições
Contribuições são bem-vindas! Se você quiser sugerir melhorias, por favor, abra um pull request ou envie uma issue no repositório.
# link colab: https://colab.research.google.com/drive/1smCSRAcn9v-eYIVt4FrClAUng1KE9bB1?usp=sharing

