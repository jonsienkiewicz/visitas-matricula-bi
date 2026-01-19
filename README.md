# 📊 Projeto de BI — Visitas de Matrícula

Este projeto simula um fluxo real de Business Intelligence em ambiente corporativo, desde a chegada de dados brutos até a definição de métricas, modelo dimensional e consumo em Power BI.

O objetivo é demonstrar capacidade analítica, organização de projeto, versionamento com Git e pensamento orientado a negócio, indo além da simples construção de dashboards.

---

## 🎯 Objetivo do Projeto

Analisar dados de visitas de matrícula realizadas em campo, respondendo perguntas de negócio como:

- Quantas visitas foram realizadas?
- Qual a taxa de conversão em matrícula?
- Quais equipes e regiões performam melhor?
- Onde existem gargalos operacionais?

---

## ❓ Perguntas de Negócio

- Quantas visitas foram realizadas por período?
- Quantas visitas resultaram em matrícula?
- Qual a taxa de conversão (%)
- Qual o desempenho por equipe, região e agente?
- Existem padrões temporais (dia, mês, período)?

---

## 📐 Métricas Definidas

- Total de Visitas
- Total de Matrículas
- Taxa de Conversão
- Visitas por Região
- Visitas por Equipe
- Matrículas por Região
- Matrículas por Equipe

---

## 🧠 Regras de Negócio

As regras de negócio são aplicadas na base tratada, incluindo:

- Normalização de datas
- Criação de flags de matrícula
- Padronização de textos
- Criação de colunas derivadas para análise
- Tratamento de dados inconsistentes

---

## 🗂 Estrutura do Projeto

visitas-matricula-bi/
├── data/
│   ├── raw/
│   │   └── visitas_matricula_bruto.csv
│   └── processed/
│       └── visitas_matricula_tratada.xlsx
├── docs/
│   ├── regras_de_negocio.md
│   ├── perguntas_de_negocio.md
│   ├── modelo_analitico_power_bi.md
│   └── modelo_dimensional.md
├── powerbi/
│   └── visitas_matricula.pbix
├── README.md
└── .gitignore

---

## 🧱 Modelo Dimensional

Fato:
- Visitas de Matrícula

Dimensões:
- Tempo
- Região
- Equipe
- Agente

---

## 📊 Power BI

Utilizado para consumo da base tratada, criação de medidas e visualização analítica.

---

## 🛠 Tecnologias Utilizadas

- Excel
- Power BI
- Git & GitHub
- Markdown
- CSV

---

## 🧩 Diferenciais

- Versionamento completo
- Documentação clara
- Separação raw/processed
- Estrutura próxima à realidade corporativa

---

## 👤 Autor

Jonathan Santos de Jesus Sienkiewicz  
Analista de Dados
