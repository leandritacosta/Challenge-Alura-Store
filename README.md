## 🚀Challenge-Alura-Store: 


   Olá! Bem-vindo(a) ao projeto de análise dos dados. Aqui, transformamos os dados brutos em insights estratégicos para guiar Sr. João na decisão de qual loja deverá vender para expandir seus negócios📈.

  # 📊 Projeto de Análise de Vendas das 4 Lojas

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=plotly)
![Status](https://img.shields.io/badge/Status-Finalizado-success)

---

## 📝 Sobre o Projeto

Este projeto tem como objetivo analisar os dados de **4 lojas** do Sr. João.  
A análise busca responder perguntas importantes, como:

- Qual loja tem o maior e menor faturamento?
- Quantos produtos foram vendidos em cada loja?
- Como estão as avaliações dos clientes?
- Quais são os produtos mais e menos vendidos?
- Qual loja apresenta maior instabilidade e deve ser vendida?

A partir de **dados reais em CSV**, utilizamos **Python, Pandas e Matplotlib** para organizar, calcular e visualizar os resultados.

---

## 📌 Sumário
- [📂 Importação dos Dados](#-importação-dos-dados)
- [💰 Faturamento das Lojas](#-faturamento-das-lojas)
- [🛒 Vendas por Categoria](#-vendas-por-categoria)
- [⭐ Média de Avaliação](#-média-de-avaliação-das-lojas)
- [🏆 Produtos Mais e Menos Vendidos](#-produtos-mais-e-menos-vendidos)
- [🚚 Frete Médio](#-frete-médio-por-loja)
- [📈 Visualização dos Gráficos](#-visualização-dos-gráficos)
- [📑 Relatório Final](#-relatório-final)
- [🛠️ Ferramentas e Tecnologias](#ferramentas-e-tecnologias)
- [📬 Contatos](#contatos)

---

## 📂 Importação dos Dados

Os dados foram disponibilizados em **arquivos CSV** contendo as informações de cada loja:

- Produto
- Categoria
- Preço
- Avaliação da compra
- Quantidade de parcelas
- Frete

Exemplo de importação:

```python
import pandas as pd

urls = [
  "loja_1.csv",
  "loja_2.csv",
  "loja_3.csv",
  "loja_4.csv"
]

dfs = [pd.read_csv(url) for url in urls]
```

## 💰 Faturamento das Lojas

O faturamento corresponde à soma total das vendas (receita).
| Loja      | Faturamento (R$)  |
| --------- | ----------------- |
| Loja 1    |    1534509.12     |
| Loja 2    |    1488459.06     |
| Loja 3    |    1464025.03     |
| Loja 4    |    1384497.58     |
| **Total** |    5871490.79     |

📌 Insights:

- A Loja 1 possui o maior faturamento.

- A Loja 4 apresenta o menor desempenho.

 ## 🛒 Vendas por Categoria
  Foi calculado a quantidade de produtos vendidos por categoria em cada loja.
  Isso permite identificar quais tipos de produtos eram mais vendidos.

📂 Exemplo - Loja 1:

| Categoria        | Quant. produtos vendidos |
| ---------------- |  ---------------------   |
| Brinquedos       |        23993.78          |
| Eletrôdomésticos |        484913.36         |
| Eletrônicos      |        572659.23         |


## ⭐ Média de Avaliação das Lojas

A média dessas avaliações mostra o nível de satisfação em cada loja.
| Loja   | Média de Avaliação |
| ------ | ------------------ |
| Loja 1 | 3.97               |
| Loja 2 | 4.03               |
| Loja 3 | 4.04               |
| Loja 4 | 3.99               |

📌 Insights:

- A Loja 3 tem a melhor avaliação média.

- A Loja 1 é a pior avaliada, mesmo sendo a de maior faturamento.

## 🏆 Produtos Mais e Menos Vendidos

A análise também identificou os produtos com maior e menor receita. 
 -🔝 Os 5 Produtos Mais Vendidos
| Loja   | Produto          | Receita (R$)  |
| ------ | ---------------- | ------------- |
| Loja 1 | TV Led UHD 4K    | 189534.28     |
| Loja 2 | Celular Plus X42 | 150967.83     |
| Loja 3 | Geladeira        | 133185.99     |
| Loja 4 | Celular Plus X42 | 128930.07     |

 -🔝 Os 5 Produtos Menos Vendidos
| Loja   | Produto          | Receita (R$)  |
| ------ | ---------------- | ------------- |
| Loja 1 | Corda de Pular   | 870.89        |
| Loja 2 | Cubo Mágico 8x8  | 858.22        |
| Loja 3 | Cubo Mágico 8x8  | 853.81        |
| Loja 4 | Corda de Pular   | 939.74        |

📌 Insights:

 - A Loja 4 aparece frequentemente nos piores desempenhos.
 - Algumas lojas possuem produtos “campeões” que sustentam parte da receita.

## 🚚 Frete Médio por Loja

O frete médio mostra o custo médio de envio dos produtos.
| Loja   | Frete Médio (R$)  |
| ------ | ----------------- |
| Loja 1 |     34.692        |
| Loja 2 |     33.622        |
| Loja 3 |     33.074        |
| Loja 4 |     31.279        |

📌 Insights:

 - A Loja 1 tem o frete mais caro em média.

 - O menor custo de frete é da Loja 4.

## 📈 Visualização dos Gráficos

Para facilitar a interpretação, foram criados gráficos de:

 - 📊 Pizza → Participação de cada loja no faturamento total

 - 📊 Barras → Comparação dos produtos mais e menos vendidos

 - 📊 Dispersão → Avaliação média por loja

## 📑 Relatório Final

📌 Principais conclusões:

- Se o critério for faturamento → a loja com menor receita total é a de pior desempenho.

- Se o critério for avaliação → a loja com menor média de notas é a de pior percepção pelo cliente.

- Se quisermos uma visão geral de desempenho → a pior loja é aquela que combina baixo faturamento, poucas vendas e baixa avaliação. 

✅ Decisão: A Loja 4 deve ser vendida, pois é a de pior desempenho no conjunto geral.

## Ferramentas e Tecnologias

  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original-wordmark.svg" width="80" height="80"/>  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original-wordmark.svg" width="80" height="80"/>  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/matplotlib/matplotlib-original.svg" width="80" height="80"/>   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/googlecolab/googlecolab-original.svg" width="80" height="80"/>


          
## 📩Contatos
Com dúvidas? Para mais informações entre em contato:
<div>
          <a href="https://www.instagram.com/leandracostaofficial?igsh=MWR0cWJiOTh4cjF6Zg==" target="_blank"><img loading="lazy" src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
         <a href="https://www.linkedin.com/in/leandritacosta" target="_blank"><img loading="lazy" src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
</div>        
          
           
                        📌 Desenvolvido por Leandra Costa, em Resolução do Challenge AluraStore - Data Science.
