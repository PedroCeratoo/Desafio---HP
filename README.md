# 🚀 Desafio Técnico | House Performance

Repositório dedicado à conclusão do desafio técnico para a vaga de Analista de BI/Dados Júnior na empresa House Performance.

## 🎯 Objetivo

Dentro de um contexto de **Marketing Digital e análise de funis de vendas**, este desafio técnico tem como foco principal aplicar conhecimentos em **ETL**, **visualização de dados**, **métricas de mídia paga** e **análise estratégica** com o intuito de **otimizar campanhas digitais**.

---

## ⏱️ Tempo estimado de execução

- ⌛ Entrega: **até 2 dias**
- ✅ Tempo gasto: **Aproximadamente 4 horas**

---

## 🧪 Tecnologias utilizadas

- Google Sheets
- Google Looker Studio
- SQL (PostgreSQL)
- Python
- Markdown & GitHub

---

## 🗂️ Estrutura do desafio

### 📍 Parte 1 – Preparação de Dados e Visualização no Looker Studio

#### 📌 Requisitos:
- Visualização de dados da planilha de mídia paga digital
- Métricas calculadas:
  - Impressões
  - Cliques
  - Leads
  - Valor Gasto
  - **CPM** = Valor Gasto / Impressões * 1000
  - **CTR** = Cliques / Impressões
  - **CPL** = Valor Gasto / Leads
  - **Taxa de Conversão** = Leads / Cliques
- Filtros:
  - Intervalo de datas
  - Campanha / Grupo de Anúncio / Canal 
- Drill-down entre Campanha → Grupo de Anúncio

#### 📊 Dashboard:

> 🔗 **[Dashboard do Desafio técnico](https://lookerstudio.google.com/reporting/c4bd0565-98cb-42b7-9c8c-d38f5d0322a5)**

<img width="1341" height="754" alt="image" src="https://github.com/user-attachments/assets/c81f177c-c7f3-4e1b-bb09-288c2c0a56b6" />

---

### 🛢️ Parte 2 – Análise SQL com Banco de Dados Local

#### 🧱 Schema utilizado:

#

A segunda etapa do desafio pedia que os dados da planilha fossem inseridos em um banco de dados local, com o objetivo de realizar análises utilizando SQL.
Foram propostas duas perguntas principais: identificar qual campanha trouxe o maior número de leads no período total e qual apresentou o melhor custo por lead (CPL).

Para isso, foi criado um schema no PostgreSQL com base na estrutura da planilha original. Em seguida, foram elaboradas consultas SQL que permitiram responder às perguntas de forma objetiva, utilizando funções agregadas e cláusulas de ordenação e filtragem.

As respostas obtidas estão acompanhadas dos prints das queries e resultados diretamente do banco, garantindo a transparência e rastreabilidade da análise realizada.

## Qual Campanha trouxe mais leads no período total

<img width="1542" height="846" alt="image" src="https://github.com/user-attachments/assets/5d6c0179-7ba2-4e72-b05f-d56ba9bbd4ae" />

## Qual Campanha tem melhor CPL no período total

<img width="1546" height="851" alt="image" src="https://github.com/user-attachments/assets/3c08da64-720e-4fc9-9b73-f736b24388cc" />



