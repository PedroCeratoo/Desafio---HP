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

<img width="1534" height="848" alt="image" src="https://github.com/user-attachments/assets/d9dc5dc0-bbe0-41ec-ae59-c0e7a5f48f17" />

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

### 🧩 FASE 2: Integrações e Python

Na última etapa do desafio técnico, foi solicitado que realizássemos a integração com uma API REST pública, a fim de coletar dados da última semana e armazená-los em uma planilha. Para isso, optei por utilizar a API pública do CoinGecko, que fornece dados históricos de preços de diversas criptomoedas sem necessidade de autenticação.

## 🌐 API Utilizada
> **Nome:** CoinGecko API
> **Documentação oficial:** https://www.coingecko.com/en/api/documentation
> **Endpoint usado:** https://api.coingecko.com/api/v3/coins/{coin}/market_chart/range

## 🐍 Lógica e Script em Python

> Define uma lista de criptomoedas para monitorar (bitcoin, ethereum, solana, ripple, cardano).
> Calcula os timestamps dos últimos 7 dias.
> Para cada moeda, consulta o histórico de preços.
> Formata os dados em uma tabela com coin, date e price_usd.
> Exporta o resultado para um arquivo CSV: precos_criptos_desafioHP.csv.

<img width="1026" height="859" alt="image" src="https://github.com/user-attachments/assets/0342e04a-5d8f-4349-b260-ff7d7f467c0a" />
# O resultado foi uma planilha com os o nome das moedas, data e hora de coleta de preço, na última semana, e os preços em dólar: (https://docs.google.com/spreadsheets/d/1bFF1f70WXiPso4YR2_w2NaW8fSiTRe--2S8huyah54I/edit?usp=sharing)


