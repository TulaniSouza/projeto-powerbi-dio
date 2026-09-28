# Desafio de Projeto: Coleta e Processamento de Dados com Power BI

Repositório dedicado ao desafio de projeto da formação Power BI Analyst, focado na integração de dados locais através do MySQL Workbench e na limpeza e transformação de dados utilizando o Power Query.

## Objetivo Geral
Configurar um banco de dados local com MySQL Workbench, popular as tabelas através de scripts SQL, integrar a base de dados com o Microsoft Power BI e realizar as transformações necessárias para a construção de relatórios consistentes.

## Etapas do Projeto

1. **Infraestrutura e Integração Local:**
   - Criação da base de dados através do MySQL Workbench.
   - Execução dos scripts SQL fornecidos para criação de tabelas e inserção de dados.
   - Ligação direta da base de dados local (localhost) ao Microsoft Power BI.

2. **Transformação de Dados (Power Query):**
   - Verificação de cabeçalhos e tipos de dados, com foco na conversão rigorosa de valores monetários para o tipo *double*.
   - Tratamento de valores nulos, identificando que a ausência de dados na coluna `Super_ssn` indica os gerentes da empresa.
   - Mescla das consultas `employee` e `department` para criar uma tabela unificada com os nomes dos departamentos associados aos respetivos colaboradores.
   - Junção de dados para associar os colaboradores aos seus gerentes.
   - Concatenação das colunas de Nome e Sobrenome para gerar uma coluna única de "Nome Completo" dos colaboradores.
   - Mescla dos nomes dos departamentos com as suas respetivas localizações para garantir combinações exclusivas.
   - Agrupamento de dados para contabilizar a quantidade de colaboradores associados a cada gerente.
   - Limpeza e otimização do modelo de dados, procedendo à remoção de colunas redundantes ou desnecessárias para o relatório final.

## Perguntas Técnicas do Desafio

**Por que na junção de departamento e localização utilizamos a função "Mesclar" e não "Atribuir/Acrescentar"?**
Neste cenário, utilizamos a função **Mesclar** (Merge) porque o objetivo é cruzar atributos de entidades complementares lado a lado (adicionando novas colunas de localização às linhas dos departamentos existentes) com base numa chave comum, de forma equivalente a um comando `JOIN` em SQL. A função **Atribuir/Acrescentar** (Append) funciona como um `UNION`, empilhando novas linhas de dados numa tabela já existente. Isto exigiria que ambas as consultas tivessem a mesma estrutura e representassem a mesma entidade, o que não se aplica à relação entre departamentos e as suas localizações.

## Diferença entre Mesclar e Acrescentar Consultas

- **Mesclar (Merge):** Realiza uma junção **horizontal** de tabelas relacionando colunas equivalentes a partir de uma chave primária/estrangeira (similar ao `JOIN` em SQL). Foi utilizado para associar localizações aos departamentos e gerentes aos colaboradores.
- **Acrescentar (Append):** Realiza uma junção **vertical** empilhando dados de tabelas que possuem estruturas semelhantes (similar ao `UNION` em SQL). Não se aplica ao cruzamento de entidades distintas como Departamento e Localização.

## Ferramentas Utilizadas
- Microsoft Power BI (Power Query)
- MySQL Workbench (Base de Dados Local)
- Visual Studio Code & Git