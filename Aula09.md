## 1. Introdução e Visão Geral
Este parecer analisa as práticas de programação assistida por IA abordadas na Unidade II. A principal conclusão é que a IA não deve ser encarada como uma substituta, mas como uma ferramenta de **aumento de capacidades**. O foco do desenvolvedor moderno desloca-se da escrita manual de sintaxe para a arquitetura de soluções lógicas e seguras.

## 2. Práticas de Workflow e Implementação
Durante os estudos, destaca-se a importância do **Desenvolvimento Guiado por Comentários**. O fluxo estabelecido em três etapas (Intenção Humana → Proposta da IA → Refinamento Humano) garante que o controle do código permaneça com o desenvolvedor.

*   **Refatoração e Manutenção:** A transição da IA de "geradora" para "analista de compreensão" é vital para lidar com código legado, permitindo documentar e analisar impactos antes de qualquer alteração.
*   **Automação de Testes:** A utilização da IA para gerar testes unitários e identificar *edge cases* aumenta a robustez do software, cobrindo falhas que muitas vezes passam despercebidas no desenvolvimento manual.

## 3. Análise Crítica: Ética, Segurança e Ferramentas
O uso de ferramentas como **GitHub Copilot, Replit e Ghostwriter** exige responsabilidade técnica e ética:

*   **Responsabilidade Legal:** Como o assistente não possui consciência, o desenvolvedor assume total responsabilidade por cada *commit*. O código deve passar por checklists de segurança contra vulnerabilidades (SQL Injection, XSS).
*   **Propriedade Intelectual:** Vigilância constante sobre as licenças de código para evitar violações em produtos comerciais.
*   **Transparência:** Em sistemas críticos, a explicabilidade é mandatória. Não se aceita uma "caixa preta" em algoritmos que impactam vidas humanas.
