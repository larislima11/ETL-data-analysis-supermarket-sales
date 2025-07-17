# 🛒 Supermarket Customer Behavior Analysis | Análise de Comportamento de Clientes de Supermercado

Este projeto é uma análise aprofundada do comportamento de compra dos clientes de um grande supermercado. Usando um pipeline completo de processamento de dados e visualização, nosso objetivo é transformar dados brutos em insights acionáveis que podem otimizar estratégias de marketing e operações.

# Objetivo

- Compreender Padrões de Compra: analisar como os clientes compram, incluindo a variação das vendas por hora e as categorias de produtos mais populares.
- Segmentar Clientes: explorar dados demográficos para identificar o perfil dos nossos consumidores.
- Gerar Insights Estratégicos: fornecer ao supermercado informações valiosas para melhorar campanhas de marketing, otimizar estoque e aprimorar a experiência do cliente.

#  Estrutura do projeto e tarefas realizadas

### 1. Geração de Dados Simulados

Para garantir um ambiente de desenvolvimento controlável e reproduzível, criei três conjuntos de dados sintéticos que mimetizam informações reais de um supermercado:

* **`vendas.csv`**: contém detalhes de cada transação, como `id_venda`, `id_produto`, `valor`, `hora_compra` e `id_cliente`.
* **`clientes.csv`**: inclui informações demográficas dos clientes, como `id_cliente`, `idade`, `gênero` e `localizacao`.
* **`produtos.csv`**: fornece detalhes dos produtos, incluindo `id_produto`, `categoria` e `preco`.

### 2. Processamento de Dados (ETL)

Essa fase crucial prepara os dados brutos para a análise:

* **Extração:** eu carrego os dados simulados diretamente dos arquivos CSV.
* **Transformação:** realizo a limpeza e o enriquecimento dos dados. Isso envolve:
    * Tratamento de valores ausentes e correção de tipos de dados (especialmente para `hora_compra`).
    * Cálculo de métricas importantes como **ticket médio por cliente** e **quantidade média de itens por compra**.
    * Derivação de novas *features* de tempo (ex: `hora`, `dia_da_semana`) a partir da `hora_compra`.
* **Carga:** os dados transformados são estruturados em um formato otimizado para análise, simulando um **Data Warehouse** com tabelas de fatos e dimensões.

### 3. Análise e Visualização

Com os dados limpos e estruturados, eu mergulho na análise e na criação de visualizações para extrair e comunicar insights:

* **Volume de Vendas por Hora do Dia (Gráfico de Linhas):**
    * *Insight:* Revela os horários de pico e de menor movimento, auxiliando na alocação de equipe e no timing de promoções.
* **Quantidade de Produtos Vendidos por Categoria (Gráfico de Barras):**
    * *Insight:* Destaca as categorias de produtos mais populares, orientando decisões de estoque e sortimento.
* **Proporção de Clientes por Faixa Etária (Gráfico de Pizza):**
    * *Insight:* Oferece uma visão demográfica da base de clientes, auxiliando no direcionamento de campanhas de marketing.

---

## Organização dos Dados

Os dados simulados são organizados da seguinte forma:

* **`clientes.csv`**:
    * `id_cliente`: Identificador único de cada cliente.
    * `idade`: Idade do cliente.
    * `gênero`: Gênero do cliente (Masculino, Feminino).
    * `localizacao`: Cidade de residência.

* **`vendas.csv`**:
    * `id_venda`: Identificador único da transação.
    * `id_produto`: Produto adquirido na venda.
    * `valor`: Valor total da venda.
    * `hora_compra`: Timestamp da transação.
    * `id_cliente`: Cliente que realizou a compra.

* **`produtos.csv`**:
    * `id_produto`: Identificador único do produto.
    * `categoria`: Categoria do produto (Alimentos, Bebidas, Eletrônicos, etc.).
    * `preco`: Preço unitário do produto.

---

## Visualizações Chave

As visualizações geradas são cruciais para a compreensão dos padrões de compra:

1.  **Gráfico de Linhas - Volume de Vendas por Hora do Dia:**
    * Este gráfico ilustra a variação do volume de vendas ao longo das 24 horas, identificando os períodos de maior e menor atividade.
      
  <img width="629" height="410" alt="image" src="https://github.com/user-attachments/assets/999f130c-fab3-4319-ab50-5fa41312edca" />

2.  **Gráfico de Barras - Quantidade de Produtos Vendidos por Categoria:**
    * Compara a popularidade das diferentes categorias de produtos (ex: alimentos vs. bebidas vs. eletrônicos), destacando as mais vendidas.
      
  <img width="644" height="428" alt="image" src="https://github.com/user-attachments/assets/0736174a-5b54-44ad-9a8e-7f48472e33e3" />

3.  **Gráfico de Pizza - Proporção de Clientes por Faixa Etária:**
    * Apresenta a distribuição percentual dos clientes em distintas faixas etárias, oferecendo insights sobre o público-alvo principal do supermercado.

<img width="446" height="451" alt="image" src="https://github.com/user-attachments/assets/a76133bb-7214-4b7f-bc8b-63c4667823aa" />

---

## Futuras Melhorias

Este projeto serve como uma base sólida, mas pode ser expandido com as seguintes melhorias:

* **Integração com Firebase:** adicionar persistência dos dados e tornar o sistema mais escalável usando um banco de dados NoSQL real, como Firebase.
* **Análise Preditiva:** implementar modelos de Machine Learning para prever o comportamento futuro dos clientes, como *churn*, valor de tempo de vida (*LTV*) ou recomendação de produtos.
* **Análise Geoespacial:** incorporar visualizações de mapa para analisar a distribuição geográfica dos clientes e identificar regiões com maior potencial de vendas.

---
# Contribuições
Contribuições são bem-vindas! Se você quiser sugerir melhorias, por favor, abra um pull request ou envie uma issue no repositório.

## 🔗 Link para o Notebook

* **Google Colab:** [https://colab.research.google.com/drive/1smCSRAcn9v-eYIVt4FrClAUng1KE9bB1?usp=sharing](https://colab.research.google.com/drive/1smCSRAcn9v-eYIVt4FrClAUng1KE9bB1?usp=sharing)

---

