
# 📊 Dashboard de Gestão de Vendas – Power BI

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
Dashboard_de_Vendas/
├── Dashboard_de_Vendas.pbix     → Arquivo principal do Power BI
├── bd_vendas.xlsx               → Base de dados de vendas e lojas
├── imagens/                     → Capturas de tela do dashboard
│   └── dashboard_vendas.png
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

## 🖼️ Captura do Dashboard

![Dashboard de Vendas](imagens/dashboard_vendas.png)

---

## 👨‍💻 Desenvolvedor

Jair Cipriano  
📧 jaircipriano69@gmail.com

---

## 📜 Licença

Projeto sob licença [MIT](LICENSE).
