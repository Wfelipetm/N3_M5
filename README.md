# Tratamento de Dados com Python e Pandas

## Descrição
Este repositório contém um exemplo prático de como limpar e preparar um conjunto de dados para análise usando Python e a biblioteca Pandas. O objetivo é demonstrar passo a passo como transformar dados brutos em um formato adequado para mineração e análise de dados.

## Contexto
Como Analista de Dados, é comum receber conjuntos de dados que precisam de preparação antes de poderem ser analisados. Este projeto simula essa situação, usando um conjunto de dados fictício composto por colunas como `ID`, `Duration`, `Date`, `Pulse`, `Maxpulse` e `Calories`.

## Passos Realizados

1. **Leitura e Verificação Inicial**
   - Leitura do arquivo CSV fornecido.
   - Verificação das informações gerais sobre os dados.
   - Impressão das primeiras e últimas linhas do arquivo para visualização inicial.

2. **Criação de uma Cópia dos Dados Originais**
   - Criação de uma cópia do dataframe original para preservar os dados brutos.

3. **Tratamento da Coluna 'Calories'**
   - Substituição de valores nulos na coluna 'Calories' por 0 para evitar inconsistências na análise posterior.

4. **Tratamento da Coluna 'Date'**
   - Substituição de valores nulos na coluna 'Date' por '1900/01/01' para padronização.

5. **Transformação da Coluna 'Date' para Formato Datetime**
   - Utilização do método `to_datetime` do Pandas para transformar a coluna 'Date' em um formato de data adequado.

6. **Correção de Formatos Específicos na Coluna 'Date'**
   - Correção de formatos específicos como "20201226" para o formato datetime usando combinação de métodos `replace` e `to_datetime`.

7. **Remoção de Registros com Valores Nulos na Coluna 'Date'**
   - Remoção de registros onde a coluna 'Date' possui valores nulos após o tratamento.

