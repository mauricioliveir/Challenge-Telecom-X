# 📊 Desafio Telecom X: Análise de Evasão de Clientes (Churn Prediction)

**Autor:** Mauricio de Oliveira  
**Última atualização:** 10/06/2025 

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 🚀 Visão Geral

Este projeto foi desenvolvido como parte de um desafio de **Data Science** para a empresa fictícia **Telecom X**, com o objetivo de identificar os principais fatores que influenciam a evasão de clientes (_churn_).

Utilizando **Python** no **Google Colab**, aplicamos análise exploratória de dados (EDA) e visualizações e para gerar insights acionáveis que ajudem a empresa a melhorar a **retenção de clientes**.

---

## 🔍 Principais Descobertas

- 👴 **Idosos** possuem uma taxa de churn de **41,7%** (vs. média geral de 26,5%).
- 📅 **Clientes com contrato mensal** são **15x mais propensos a cancelar** do que os com contrato bienal.
- 💻 **Usuários de fatura digital** apresentam **33,6% de churn**, quase o dobro em comparação aos de fatura impressa (16,3%).

---

## 📁 Estrutura do Projeto

O projeto foi desenvolvido em um único notebook no **Google Colab**.

### 📥 Importação de Dados  
#### Fonte dos dados:
[TelecomX_Data.json](https://raw.githubusercontent.com/alura-cursos/challenge2-data-science/refs/heads/main/TelecomX_Data.json).

### 🧹 Pré-processamento  
- Tratamento de valores ausentes (NaN).  
- Conversão de variáveis categóricas (ex: `gênero`, `tipo_contrato`).

### 📊 Análise Exploratória (EDA)  
- Visualizações com **Matplotlib** e **Seaborn**.  
- Análise de **correlação entre variáveis**.

### 💡 Extração de Insights  
- Identificação dos grupos com maior risco de cancelamento.  
- Comparações entre tipos de contrato, faixa etária e métodos de pagamento.

---

## 📌 Recomendações Estratégicas

✅ Ações sugeridas com base nos dados:

- 💬 Incentivar a **migração de contratos mensais para anuais/bienais** com benefícios.  
- 👵 Criar **planos exclusivos para clientes idosos** (ex: atendimento prioritário).  
- 📲 **Otimizar a experiência de fatura digital** (ex: envio por WhatsApp, interface simplificada).

---

## 🔍 Sobre o Dataset

| Característica       | Descrição                                                    |
|----------------------|--------------------------------------------------------------|
| **Fonte**            | Dados sintéticos simulando uma operadora de telecom (2023).  |
| **Tamanho**          | ~10.000 registros                                             |
| **Variáveis**        | 20+ colunas (idade, contrato, dependentes, etc.)             |
| **Target**           | `churn` (binário: 0 = ativo, 1 = cancelado)                  |

---

## 📈 Principais Visualizações

### 🔹 Distribuição de Churn por Idade  
> Pico de evasão entre clientes acima de 60 anos.

```python
sns.histplot(data=df, x='idade', hue='churn', bins=30)
```

---

### 🔹 Impacto do Tipo de Contrato  
> Contratos mensais apresentam churn de **42,7%** vs. **2,8%** em contratos bienais.

---

### 🔹 Fatura Digital x Fatura Impressa  
> Churn de **33,6%** com fatura digital vs. **16,3%** com fatura impressa.

---

## ⚙️ Tecnologias Utilizadas

- **Linguagem:** Python  
- **Bibliotecas:**
  - `Pandas` – manipulação de dados
  - `Numpy` – para computação numérica
  - `Seaborn` / `Matplotlib` – visualizações
- **Ambiente:** Google Colab

---

## 🛠️ Como Reproduzir a Análise

1. Acesse o notebook no Colab:  
🔗 _[Link para o Notebook no Google Colab](https://colab.research.google.com/drive/1j98-o8r4OuxOjNzv-oxEne8s-aHbXk0-#scrollTo=_ajJOezKULQt)_

2. Execute todas as células sequencialmente.

---

## 🤝 Contato

📧 **Email:** [GMail](malito:manutencaomauricio81@gmail.com) 
🔗 **LinkedIn:** [Mauricio De Oliveira](https://www.linkedin.com/in/monitormauricio/)
