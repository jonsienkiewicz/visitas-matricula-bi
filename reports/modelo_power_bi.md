# Modelo Analítico – Power BI

Este documento descreve como os dados tratados devem ser consumidos
no Power BI para construção dos dashboards operacionais.

---

## 1. Fonte de Dados

- Origem: Excel
- Arquivo: data/processed/visitas_matricula_tratadas.xlsx
- Aba: base_tratada

A tabela `base_tratada` deve ser importada como tabela fato única
para este dashboard.

---

## 2. Grão dos Dados

- 1 linha representa 1 visita de matrícula realizada em campo

Todas as métricas devem respeitar esse grão.

---

## 3. Medidas (DAX)

### Total de Visitas
```DAX
Total Visitas = COUNT(base_tratada[id_visita])
