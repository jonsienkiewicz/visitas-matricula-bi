# Modelo Dimensional – Visitas de Matrícula

Este documento descreve o modelo analítico proposto para análise das visitas de matrícula,
independente da ferramenta de BI utilizada.

## Tabela Fato: fato_visitas

Grão da tabela:
- Uma linha por visita realizada

Principais métricas:
- Quantidade de visitas
- Quantidade de visitas válidas
- Quantidade de visitas com status CAPTADO
- Quantidade de visitas que seguem para CAPEX

## Dimensão Tempo: dim_tempo
- data_visita
- dia
- mês
- ano

## Dimensão Localidade: dim_localidade
- bairro

## Dimensão Status da Visita: dim_status
- status_normalizado
- fluxo

## Dimensão Instalação: dim_instalacao
- flag_instalacao_hidrometro
