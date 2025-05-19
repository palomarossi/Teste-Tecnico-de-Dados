# 📊 Análise do E-Commerce Brasileiro (Olist)

*Análise exploratória e insights sobre o dataset Brazilian E-Commerce da Olist no Kaggle. O projeto inclui processamento de dados, visualizações e modelos preditivos.*

![Badge Status](https://img.shields.io/badge/status-concluído-success)
![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/pandas-1.3+-orange)
![License](https://img.shields.io/badge/license-MIT-green)

🔗 **Dataset Original**: [Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## 🌟 Principais Análises
- **Comportamento de Compra**: Sazonalidade e ticket médio por estado
- **Avaliação de Clientes**: Relação entre tempo de entrega e notas de avaliação
- **Performance de Vendedores**: Média de tempo para envio por região
- **Modelo Preditivo**: Previsão de atrasos nas entregas (Logistic Regression)

---

## 🛠 Tecnologias Utilizadas
**Análise de Dados:**
- Python 3.9
- Pandas
- NumPy
- Matplotlib/Seaborn

**Machine Learning:**
- Scikit-learn

**Ferramentas:**
- Google Colab
- Git
---

## ⚙️ Estrutura do Dataset
O dataset contém:
- `olist_orders_dataset.csv` (dados de pedidos)
- `olist_order_items_dataset.csv` (itens dos pedidos)
- `olist_customers_dataset.csv` (dados de clientes)
- +8 tabelas relacionadas

## **Preparação dos Dados**

Carregamento: Todos os datasets foram carregados em DataFrames pandas.

Conversão de Datas: Colunas de timestamp foram convertidas para o tipo datetime para análise temporal.

Tratamento de Nulos: Valores ausentes em datasets como orders, products e order_reviews foram tratados com remoção ou preenchimento estratégico.

Remoção de Duplicatas: Registros duplicados em customers, sellers, products, order_items e geolocation foram removidos para garantir a unicidade dos dados.

Normalização de Texto: Nomes de categorias de produtos foram padronizados (minúsculas, remoção de underscores/espaços).

Agregação de Geolocalização: Coordenadas geográficas foram agregadas pela média por prefixo de CEP.

Tradução de Categorias: As categorias de produtos foram mescladas com suas traduções para o inglês para análise unificada.

## **Modelo Relacional e Funções Auxiliares**

O projeto reconhece a estrutura relacional dos dados, permitindo a combinação de informações de diferentes tabelas (pedidos, clientes, produtos, etc.). Uma função haversine foi implementada e refinada para calcular distâncias geográficas precisas entre clientes e vendedores, considerando arredondamentos.

## **Análise Exploratória de Dados**

**Volume de Pedidos por Mês e Sazonalidade:** Análise temporal do volume de pedidos, identificando picos como a Black Friday e tendências de crescimento.

**Distribuição do Tempo de Entrega:** Avaliação do tempo que leva para os pedidos chegarem aos clientes, identificando a concentração das entregas e a presença de caudas longas para entregas mais demoradas.

**Relação entre Frete e Distância:** Análise da correlação entre o valor do frete e a distância de entrega, demonstrando a influência da distância no custo, mas também a presença de outros fatores.

**Categorias de Produtos Mais Vendidas (Faturamento):** Identificação das categorias que mais contribuem para a receita, fornecendo insights para gestão de estoque e marketing.

**Estados com Maior Valor Médio de Pedido:** Análise geográfica para identificar as regiões com maior gasto médio por pedido.

---
## 🚀 Como Executar
1. **Baixe o dataset** do [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
2. **Clone o repositório**:

---
Desenvolvido por Paloma Rossi
📧 palomarossi@gmail.com 
```bash

git clone https://github.com/palomarossi/Teste-Tecnico-de-Dados.git


