# Projeto Módulo 3 – Low Code/No Code/Vibecode

## 📌 Desafio Escolhido
Desenvolvi um **Painel Automatizado e Relacional de Gestão de Projetos e Custos para Agências de Marketing Digital**. O objetivo do sistema é organizar o fluxo de demandas de criação de conteúdo e, simultaneamente, monitorar a lucratividade dos clientes e o custo operacional de cada tarefa através de inteligência artificial e banco de dados interconectado, eliminando qualquer necessidade de codificação tradicional.

---

## 🖥️ Protótipo
* **Link de acesso:** [Painel de Gestão e Controller no Airtable](https://airtable.com)
* **Funcionamento:** O ecossistema é composto por três tabelas conectadas:
  1. **Demandas:** Gerencia o fluxo operacional e centraliza a análise da IA.
  2. **Clientes:** Controla os contratos mensais e consolida as horas totais trabalhadas.
  3. **Timesheet:** Registra os apontamentos diários de horas e calcula o custo de cada profissional.
  
O campo nativo de IA (`Attachment Summary`) cruza os dados relacionais entre as tabelas de forma autônoma. Ele gera diagnósticos em tempo real sobre a saúde do escopo e o custo financeiro acumulado de cada entrega.

> Coloque os arquivos de imagem ou PDF na pasta `/docs`.

---

## ⚙️ Plataforma Utilizada
* **Plataforma:** Airtable.
* **Justificativa da escolha:** O Airtable foi selecionado por permitir a criação de um banco de dados relacional (com chaves estrangeiras e vínculos um-para-muitos) associado a recursos nativos de IA Generativa. A plataforma permitiu estruturar cálculos financeiros complexos (como fórmulas de multiplicação e agregadores de soma *Rollup*) sem escrever uma única linha de código tradicional.

---

## ✅ Vantagens Identificadas
Com base no desenvolvimento prático e autônomo, identifiquei as seguintes vantagens:
1. **Arquitetura Relacional Sem Código:** Criação de vínculos e junções complexas entre três tabelas distintas de forma visual e imediata.
2. **Análise de Dados Avançada via IA:** A inteligência artificial provou ser capaz de realizar consultas transversais, lendo registros contidos em tabelas vinculadas (`Timesheet`) para gerar resumos de custos na tabela principal (`Demandas`).
3. **Cálculos Automatizados em Tempo Real:** Automação total do cálculo de rentabilidade através de funções de *Rollup* e *Formulas* matemáticas integradas.

---

## ⚠️ Limitações do Sistema e Erros Comuns de Usuários
Durante o desenvolvimento e modelagem da Fase 2, mapeei restrições técnicas da inteligência artificial relacional e falhas operacionais de atenção cometidas por usuários:

### Restrições Técnicas da IA
1. **Dependência de Vínculos Estruturados:** A IA não consegue deduzir custos se o usuário esquecer de criar o relacionamento físico (link) entre a linha da demanda e a linha do timesheet.
2. **Sensibilidade a Dados Nulos:** O sistema recusa o processamento e aponta erro de execução se os campos essenciais de cálculo (como valor da hora ou horas trabalhadas) estiverem vazios.

### Erros Humanos Comuns (Falta de Atenção)
1. **Falha de Salvamento no Status:** O usuário digita uma nova opção de status nas configurações da coluna, mas fecha a janela antes de apertar "Enter" para salvar. Como o campo fica vazio ou com grafia errada, a lógica condicional da IA falha ao tentar ler a célula.
2. **Confusão de Inputs (Entradas Trocadas):** Na pressa do preenchimento diário, o usuário cola o texto descritivo do projeto dentro da coluna de "Responsável" (campo configurado para e-mails/usuários). O Airtable bloqueia a colagem inválida, deixando o campo em branco, o que impede a IA de processar o plano de ação.

---

## 📚 Reflexão Crítica
A evolução do protótipo para um sistema de tabelas múltiplas trouxe o desafio de manter a interface limpa e a IA precisa. Para otimizar o espaço visual, utilizei campos ocultos e engenharia de prompt restritiva, forçando a IA a entregar análises financeiras em blocos de texto extremamente concisos.

Diante dos testes de relacionamento, a experiência prática provou que ferramentas no-code exigem uma disciplina de modelagem de dados idêntica ao desenvolvimento de softwares tradicionais. O sucesso da automação não depende apenas da capacidade da inteligência artificial, mas sim da consistência estrutural das chaves e vínculos que interconectam o banco de dados.

---

## 👥 Colaboração
Trabalho realizado de forma **individual**. Gerenciei de forma integrada e autônoma todo o ciclo de desenvolvimento: desde o desenho da arquitetura relacional, normalização das tabelas de clientes e timesheet, implementação de fórmulas matemáticas, engenharia de prompt avançada e validação dos fluxos econômicos.

---

## 🧪 Validação dos Testes Práticos (Resultados do Sistema Relacional)
O funcionamento do ecossistema avançado foi validado com sucesso através do cruzamento automático das tabelas de `Demandas` e `Timesheet`:

* **Cenário de Análise Gerada pela IA:**
  * *Entrada Operacional:* Demanda em status "In progress".
  * *Vínculo Relacional:* 3 registros de horas associados na tabela Timesheet somando R$ 150,00 de custo técnico.
  * *Retorno Diagnóstico da IA:* 
    * **Saúde do Escopo:** Demanda em andamento com consumo de horas dentro do limite planejado para a atividade de criação.
    * **Custo Operacional:** R$ 150,00 acumulados e investidos nesta demanda até o momento.

---

## 📝 Registro da Aula
* **Data:** 15/05/2026
* **Atividade:** Discussão crítica + mini-projeto de aplicação
* **Local:** Laboratório de informática 8
* **Professor(a):** Kadidja Valéria

---

## 🚀 Próximos Passos
* **Melhorias do protótipo:** Criar um painel visual de gráficos nativo do Airtable (*Interfaces*) para expor a lucratividade líquida de cada cliente de forma visual para a diretoria.
* **Evoluções para o Projeto Final da Unidade 3:** Integrar a tabela de Timesheet a um bot de Telegram ou Slack via Make/Zapier, permitindo que os designers batam o ponto de horas por comando de voz no chat, alimentando o Airtable automaticamente.

## ⚙️ Etapa 2: Desenvolvimento do Mini-Projeto de Aplicação

O protótipo funcional foi desenvolvido no laboratório utilizando uma arquitetura relacional baseada em três tabelas integradas, permitindo o cruzamento de escopo operacional com métricas financeiras.

### Lógica de Telas e Fluxo de Dados:
1. **Entrada de Dados (Timesheet):** O desenvolvedor realiza o apontamento de horas e custos por tarefa.
2. **Processamento Relacional (Demandas):** A tabela central conecta o projeto ao cliente e aciona o motor de inteligência artificial nativo do Airtable.
3. **Consolidação Gerencial (Clientes):** Fórmulas de agregação (Rollup) somam o esforço total despendido por contrato de forma automatizada, calculando a saúde financeira do projeto.

