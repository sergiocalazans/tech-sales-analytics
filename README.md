# Tech Sales Analytics

Este projeto consiste em um pipeline de **Análise de Dados e ETL** (Extração, Transformação e Carga) voltado para o setor de varejo de tecnologia. O objetivo é unificar bases de dados distintas, tratar inconsistências e gerar insights sobre o faturamento de lojas, performance de gerentes e métricas regionais.

## 📊 O Projeto

A análise utiliza dados de vendas de produtos como iPhones, Notebooks e periféricos, cruzando informações de faturamento com metas estabelecidas para diferentes regiões do Brasil.

### Principais Etapas (ETL):

1.  **Extração:** Carregamento de múltiplas fontes de dados (CSV e Excel) contendo históricos de vendas globais e regionais.
2.  **Transformação:**
    - Padronização de nomes de lojas e produtos (limpeza de strings).
    - Tratamento de valores ausentes (NaN) e inconsistências de caixa alta/baixa.
    - Criação de novas métricas, como faturamento total por pedido.
3.  **Carga/Análise:** Consolidação dos dados para visualização de metas e performance por loja.

## 📂 Estrutura de Dados

O projeto utiliza os seguintes arquivos:

- **`analise.ipynb`**: Notebook Jupyter contendo todo o código de tratamento, limpeza com a biblioteca `pandas` e visualizações.
- **`vendas_tech.csv`**: Base principal com o histórico de vendas, produtos e clientes.
- **`vendas_loja_curitiba.csv`**: Dados específicos da unidade regional Sul.
- **`gerentes_lojas.xlsx`**: Tabela de referência relacionando gerentes, lojas e suas respectivas metas mensais.

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas**: Manipulação e tratamento de dados.
- **NumPy**: Operações matemáticas e suporte a arrays.
- **Jupyter Notebook**: Ambiente para análise exploratória.

## 📈 Insights Gerados

O sistema permite identificar:

- Quais lojas estão batendo as metas mensais.
- Os produtos com maior volume de saída e ticket médio.
- A performance comparativa entre vendas presenciais e online.
- Ranking de faturamento por região (Sul, Sudeste, Nordeste, etc.).

## 🚀 Como Executar

1.  Certifique-se de ter o Python e o Jupyter instalados.
2.  Instale as dependências necessárias:
    ```bash
    pip install pandas numpy openpyxl
    ```
3.  Abra o arquivo `analise.ipynb` no seu ambiente Jupyter e execute as células em ordem para visualizar o processamento dos dados.

---

_Este projeto demonstra a aplicação de Python para automação de relatórios gerenciais e inteligência de mercado._
