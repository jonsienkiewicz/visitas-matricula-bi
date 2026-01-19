# Regras de Negócio – Visitas de Matrícula

Este documento descreve as regras aplicadas aos dados de visitas
realizadas pelas equipes de responsabilidade social durante o processo
de matrícula de novos clientes.

---

## 1. Status da Visita

Cada visita realizada em campo pode assumir um dos seguintes status:

- **SUCESSO**
  - Morador presente
  - Dados completos coletados
  - Matrícula apta a seguir para o fluxo de CAPEX

- **AUSENTE**
  - Imóvel fechado ou sem responsável no momento da visita
  - Não há coleta de dados pessoais
  - Não segue para CAPEX

- **RECUSA**
  - Morador presente, porém recusou fornecer dados
  - Não segue para CAPEX

---

## 2. Visita Realizada

Uma visita é considerada realizada quando o status é diferente de
`AUSENTE`.

- `visita_realizada_flag = 1` quando status ≠ AUSENTE
- `visita_realizada_flag = 0` quando status = AUSENTE

---

## 3. Captação com Sucesso

A captação é considerada bem-sucedida quando:

- status = `SUCESSO`

Nestes casos:
- `captacao_sucesso_flag = 1`
- Os dados do responsável e das unidades familiares são válidos

---

## 4. Fluxo para CAPEX

A matrícula segue para o time de CAPEX quando:

- status = `SUCESSO`

Regra:
- `segue_capex_flag = 1` quando status = SUCESSO

---

## 5. Unidades Familiares

- A quantidade de unidades familiares só é considerada quando a visita
  tem status `SUCESSO`
- Visitas com status `AUSENTE` ou `RECUSA` não entram na contagem

---

## 6. Indicadores-Chave (KPIs)

A partir dessas regras, os principais indicadores são:

- Total de visitas realizadas
- Taxa de sucesso na captação
- Taxa de perda por ausência
- Taxa de perda por recusa
- Total de matrículas encaminhadas para CAPEX
- Total de unidades familiares incorporadas
