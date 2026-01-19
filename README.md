# Projeto BI – Visitas de Matrícula e Fluxo CAPEX

Este projeto simula um fluxo real de dados em uma empresa de saneamento,
desde a captação em campo até a visualização em Power BI.

## Fluxo
CSV bruto → Excel (tratamento) → Power BI

## Contexto
Visitas realizadas por equipes de responsabilidade social para matrícula
de novos clientes em áreas sem saneamento.

## Indicadores
- Taxa de sucesso na captação
- Motivos de perda (ausente / recusa)
- Matrículas encaminhadas para CAPEX
- Quantidade de unidades familiares incorporadas

## Como reproduzir no Power BI
1. Conectar ao arquivo Excel em data/processed
2. Usar a aba base_tratada
3. Criar medidas conforme reports/modelo_power_bi.md
