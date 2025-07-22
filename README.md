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

> 🔗 **![Clique aqui para acessar o Dashboard no Looker Studio]([https://lookerstudio.google.com/reporting/c4bd0565-98cb-42b7-9c8c-d38f5d0322a5])**

#### 🖼️ Visual do Dashboard:

![Dashboard Screenshot](<img width="1567" height="875" alt="image" src="https://github.com/user-attachments/assets/d15d1ad0-6ea6-451f-86bd-63413f75ae19" />
)

---

### 🛢️ Parte 2 – Análise SQL com Banco de Dados Local

#### 🧱 Schema utilizado:
```sql
CREATE TABLE midia_paga (
    canal TEXT,
    campanha TEXT,
    grupo_anuncio TEXT,
    data DATE,
    impressoes INTEGER,
    cliques INTEGER,
    leads INTEGER,
    valor_gasto FLOAT
);
