# Desafio de Projeto: Modelagem Dimensional - Star Schema

Este repositório contém a entrega do desafio de projeto de criação de um modelo dimensional (Star Schema) a partir de um modelo relacional fornecido pela DIO (Digital Innovation One).

## Objetivo do Desafio
Criar um diagrama dimensional no formato Star Schema com foco na análise de dados dos **Professores**[cite: 10, 11]. 

## O que foi desenvolvido
O modelo foi construído utilizando a ferramenta MySQL Workbench e reflete o contexto de atuação dos professores nas universidades[cite: 9]. O esquema foi desenhado da seguinte forma:

### Tabela Fato
* **Fato_Professor**: Centraliza o contexto de análise, armazenando as chaves estrangeiras das dimensões e as métricas (fatos) como `Carga_Horaria` e `Qtd_Turmas`[cite: 9].

### Tabelas Dimensão
As tabelas dimensão guardam os detalhes relacionados ao contexto do professor[cite: 10]:
* **Dim_Professor**: Dados do professor, como Nome e Titulação[cite: 9].
* **Dim_Departamento**: Informações do departamento ao qual o professor pertence (Nome, Campus, Coordenador)[cite: 9].
* **Dim_Curso**: Cursos onde o professor atua[cite: 9].
* **Dim_Disciplina**: Disciplinas ministradas[cite: 9].
* **Dim_Data**: Dimensão adicionada para possibilitar análises temporais (oferta de disciplinas, etc.), contendo Dia, Mês e Ano[cite: 9, 10].

*Observação:* Conforme os requisitos do desafio, dados referentes a alunos não foram incluídos nesta modelagem[cite: 10].

## Arquivos do Projeto
* `Desafio de modelagem - Dio modulo 5.png`: Imagem exportada do diagrama Star Schema final.
* `star_schema.mwb`: Arquivo do projeto original do MySQL Workbench.

## Tecnologias Utilizadas
* MySQL Workbench
* Modelagem de Dados Dimensional