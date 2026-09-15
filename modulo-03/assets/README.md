# 🎯 Módulo 3 — Relatório Executivo e Recursos Avançados no Power BI

Este repositório contém a entrega do **Módulo 3** do Desafio de Projeto da formação **Power BI Analyst (DIO)**. O foco principal desta etapa foi o redesenho de UI/UX da Página 3, a implementação de técnicas avançadas de navegação e a otimização visual para tomada de decisão.

---

## 🚀 Destaques e Refatorações da Página 3

### 1. Substituição Estratégica de Visual (Pizza $\rightarrow$ Barras Horizontais)
* **Problema Encontrado:** O gráfico de pizza oculta valores negativos e mascara fatias irrelevantes, impedindo a visualização de prejuízos operacionais.
* **Solução:** Substituição por **Gráfico de Barras Horizontais Clusterizadas**, evidenciando com clareza o **prejuízo do segmento *Enterprise*** (projetado para a esquerda do eixo zero) e a dominância do segmento *Government*.

### 2. Navegação Dinâmica com Indicadores (Bookmarks & Seleção)
* **Otimização de Espaço:** Criação dos botões interativos **Visão Lucro** e **Visão Vendas**.
* **Mapeamento:** Alternância instantânea da camada do mapa geográfico no mesmo contêiner da tela sem necessidade de carregar novos visuais.

### 3. Cabeçalho Executivo Limpo & KPIs
* **Métricas Principais:** Destaque para os cartões de **Lucro Total (16,89 Mi)** e **Total de Vendas (118,73 Mi)**.
* **Filtro Temporal:** Segmentador por intervalo de datas simplificado (sem título de cabeçalho redundante), mantendo a identidade visual do topo padronizada com a DIO.

---

## 🖼️ Visualização da Página 3 Refatorada

![Página 3 - Dashboard Executivo](assets/pagina3.png)

---

## 📁 Arquivos do Módulo

* 📊 **[Arquivo Fonte Fonte (.pbix)](./relatorio-executivo-financials.pbix)**
* 📄 **[Relatório Exportado em PDF](./relatorio-executivo-financials.pdf)**

---

> **Nota sobre o Power BI Service:** Devido às restrições de licença corporativa/estudantil para publicação no Power BI Service, a entrega está documentada de forma completa via arquivo interativo `.pbix`, exportação `.pdf` e evidências visuais neste repositório.