# Módulo 06 - Projeto 01: Atualização de Relatório Financeiro com Foco em UX

Este repositório contém a entrega refatorada do primeiro desafio do Módulo 06 da **Formação Power BI Analyst da DIO**, com foco na melhoria da experiência do usuário (UX), design de interfaces e boas práticas de visualização de dados aplicadas a relatórios executivos.

---

## Objetivo do Desafio
Modificar o relatório financeiro original criado nas etapas anteriores, aplicando conceitos avançados de arquitetura de informação e design visual para facilitar a tomada de decisão gerencial, considerando:
* **Posicionamento e Hierarquia Visual:** Respeito ao fluxo natural de leitura (padrão em "Z") e alinhamento de métricas-chave no canto superior esquerdo.
* **Proporção Áurea e Simetria:** Equilíbrio visual das "baias" e distribuição harmoniosa dos gráficos para evitar sobrecarga cognitiva.
* **Contraste e Estética:** Uso intencional de cores, fontes legíveis e criação de espaços em branco (*whitespace*) adequados.
* **Navegabilidade Global:** Implementação de menus laterais verticais com estados visuais dinâmicos.

---

## Principais Melhorias Implementadas
1. **Menu de Navegação Lateral (Vertical):** Substituição de botões dispersos por um navegador de páginas integrado na lateral esquerda.
2. **Estados Dinâmicos de Botões:** Configuração avançada de estilo para os estados *Padrão (Default)*, *Focalizar (Hover)* e *Selecionado (Selected)*, garantindo clareza imediata sobre a página ativa.
3. **Redução de Páginas Excedentes:** Ocultação de páginas de rascunho (*Details*), consolidando o relatório final estritamente nas **3 páginas principais** exigidas pelo escopo (*Sales*, *Profit* e *Report*).
4. **Refinamento de Layout e Acessibilidade:** Ajuste de margens, respiro entre os visuais e correção de contraste em eixos e filtros.

---

## Estrutura de Arquivos
* `relatorio_financeiro_ux.pbix` — Arquivo principal do Power BI com o dashboard refatorado.
* `README.md` — Documentação técnica do projeto.
* `screenshots/` — Capturas de tela demonstrando o resultado final das páginas.