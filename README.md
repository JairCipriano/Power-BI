
# 📊 Projetos de Análise de Dados com Power BI

Este repositório reúne projetos de visualização de dados desenvolvidos no **Power BI**, com foco em processos de **ETL**, **análise exploratória** e **criação de dashboards interativos**. Cada projeto tem um objetivo específico, conjunto de dados próprios e abordagens distintas para apresentar insights relevantes por meio de gráficos, indicadores e segmentações.

---

## 📚 Conteúdo

- [📈 Projeto 1: Dashboard de Gestão de Vendas](#-dashboard-de-gestão-de-vendas--power-bi)
- [🚗 Projeto 2: Dashboard de Carros (ETL + PostgreSQL)](#-dashboard-de-carros)

---

# 📈 Dashboard de Gestão de Vendas – Power BI

## 📝 Descrição
Este projeto tem como objetivo apresentar um dashboard interativo no Power BI para análise de vendas de uma empresa fictícia. O relatório permite acompanhar indicadores como faturamento total, ticket médio, comissão, além de análises por loja, forma de pagamento, período e produtos.

---

## 🎯 Objetivos

- Monitorar o desempenho de vendas por unidade (loja)
- Identificar os produtos mais vendidos e suas representatividades
- Avaliar o desempenho mensal de faturamento
- Visualizar formas de pagamento mais utilizadas
- Acompanhar KPIs como ticket médio e valor comissionado

---

## 📁 Estrutura dos Arquivos

```
power_bi/
│
│── Dashboard_de_Vendas/
│   ├── Dashboard_de_Vendas.pbix     → Arquivo principal do Power BI
│   ├── bd_vendas.xlsx               → Base de dados de vendas e lojas
│   ├── imagens/                     → Capturas de tela do dashboard
│        └── dashboard_vendas.png
│ 
├── LICENSE                      → Licença do projeto
└── README.md                    → Este arquivo de documentação
```

---

## 🗃️ Fonte de Dados

**Arquivo Excel**: `bd_vendas.xlsx`  
Contém duas tabelas principais:

- **lojas**  
  - `codigo_loja`, `nome_loja`, `cidade`, `UF`

- **registroVendas**  
  - `ID Pedido`, `Código Loja`, `Data Pedido`, `Produto`, `Pagamento`, `Preços`, `Quantidades`, `Valor da venda`, `comissao`

---

## 📈 Visualizações Criadas

- **Cartões de KPI**: Valor faturado, Comissão, Ticket médio
- **Gráfico de colunas**: Faturamento por Loja
- **Gráfico de pizza**: Faturamento por forma de pagamento
- **Gráfico de colunas por mês**: Faturamento por período (jan–dez)
- **Tabela dinâmica**: Análise por produto (com % de participação)
- **Segmentador**: Filtro por produto (ex: Mala, Bolsa, Tênis...)

---

## ▶️ Como Usar

1. Baixe os arquivos `.pbix` e `bd_vendas.xlsx`.
2. Abra o `Dashboard_de_Vendas.pbix` com o Power BI Desktop.
3. Se necessário, atualize o caminho da planilha Excel.
4. Clique em "Atualizar" para visualizar os dados.
5. Explore os filtros e gráficos interativos.

---

## 👨‍💻 Desenvolvedor

Jair Cipriano  
📧 jaircipriano69@gmail.com

---

## 📜 Licença

Projeto sob licença [MIT](LICENSE).

---

# 🚗 Dashboard de Carros

## 📝 Descrição
Este projeto apresenta um painel de controle (dashboard) para análise de dados automotivos. O pipeline completo de **ETL** foi realizado: desde arquivos CSV até o banco de dados **PostgreSQL**, com visualização final no **Power BI**.

---

## 🔗 Estrutura do Projeto

```
power_bi/
│
├── Dashboard_de_carros/
|   |── dados/
│   |       ├── Insurance_data.csv
│   |       ├── Owners_data.csv
│   |       ├── Sales_data.csv
│   |       └── Service_History.csv
|   |──imagens/
|   |        └── Dashboard_carros.png
│   └── Projeto_E.T.L.pbix
│
├── LICENSE
└── README.md
```

---

## 📁 Fontes de Dados

- **Car_Data.csv**: Informações técnicas e gerais dos veículos.
- **Insurance_data.csv**: Dados de seguros dos carros, incluindo número da apólice e validade.
- **Owners_data.csv**: Informações dos proprietários, tipo de dono e contatos.
- **Sales_data.csv**: Dados das vendas como data, valor e comprador.
- **Service_History.csv**: Histórico de manutenção dos veículos.

---

## ⚙️ Processo ETL

1. **Extração**:
   - Dados importados dos arquivos `.csv`.

2. **Transformação**:
   - Análise e verificação prévia no **Microsoft Excel**.
   - Padronização de formatos (datas, números).
   - Tratamento de dados no Power BI com **DAX** e Power Query.

3. **Carga**:
   - Inserção dos dados em um banco de dados **PostgreSQL**.
   - Conexão do banco de dados ao Power BI.

---

## 📌 KPIs no Dashboard

- 🚘 **Total de Carros**: 25,02 mil
- 💵 **Valor Total das Vendas**: R$ 649,32 mil
- 🏷 **Marcas de Carro**: 10
- ⛽ **Tipos de Combustíveis**: 5
- 🌆 **Total de Cidades**: 10

---

## 📈 Visões Apresentadas

- **Distribuição por Tipo de Combustível** (barra horizontal)
- **Vendas Anuais** (colunas por ano)
- **Total de Carros por Marca** (gráfico de rosca)
- **Transmissão Manual vs Automática** (gráfico de rosca)

---

## 🎨 Layout

- Tema: **Azul e Branco**
- Cores principais: Tons de azul para destaque visual
- Gráficos com dados bem distribuídos e legibilidade aprimorada
- Estilo limpo, profissional e moderno

---

## 🧠 Ferramentas Utilizadas

- **Power BI** (Modelagem, visualização, DAX)
- **PostgreSQL** (Banco de dados relacional)
- **Excel** (Pré-análise dos dados)
- Linguagem **DAX** e **Power Query**
