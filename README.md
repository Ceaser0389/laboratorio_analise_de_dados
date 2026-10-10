# 📊 Análise de Vendas com Excel e Python

Projeto de análise de dados que explora uma base de 2.359 vendas (jan/2020 a mar/2023), responde seis perguntas de negócio e apresenta os resultados em um dashboard no Excel e em um notebook Jupyter com Python (`pandas` e `matplotlib`).

---

## 🎯 Objetivo

Transformar uma base bruta de vendas em informação útil para decisão, respondendo:

* Qual categoria possui o maior faturamento?
* Qual estado possui a maior quantidade de vendas?
* Qual é o produto mais vendido?
* Qual forma de pagamento é mais utilizada?
* Como o volume de vendas varia ao longo dos anos?
* Qual categoria possui a menor avaliação média?

---

## 🗂️ A base de dados

* **Arquivo:** `base_vendas_voluntarios__1_.csv`
* **Volume:** 2.359 linhas · 12 colunas · sem valores vazios nem duplicatas.

| Coluna | Descrição |
| :--- | :--- |
| **Produto** | Nome do produto (51 produtos) |
| **Categoria do Produto** | Categoria (8 categorias) |
| **Preço** | Valor do produto (R\$) |
| **Frete** | Valor do frete (R\$) |
| **Data da Compra** | Data da venda (dd/mm/aaaa) |
| **Vendedor** | Vendedor responsável (14 vendedores) |
| **Local da compra** | UF da compra |
| **Avaliação da compra** | Nota de 1 a 5 |
| **Tipo de pagamento** | Cartão de crédito, boleto, cupom ou cartão de débito |
| **Quantidade de parcelas** | De 1 a 24 |
| **lat / lon** | Coordenadas da UF (não usadas na análise) |

> **Premissa:** Faturamento = soma da coluna `Preço` (o frete não entra). Cada linha da base é uma venda.

---

## 📁 Estrutura do repositório

```text
.
├── README.md
├── dashboard.png                    # imagem do dashboard
├── base_vendas_voluntarios__1_.csv  # base de dados original
├── analise_vendas.xlsx              # planilha com dashboard, tabelas e verificações
├── analise_vendas_excel.ipynb       # notebook Jupyter com as análises em Python
└── analise_financeira_vendas.py     # script de exploração das colunas financeiras
