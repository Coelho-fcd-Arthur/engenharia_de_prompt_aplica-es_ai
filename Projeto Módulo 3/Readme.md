# Projeto Módulo 3 – Low Code/No Code/Vibecode

## 📌 Desafio Escolhido
Desenvolvi um **Painel Automatizado de Gestão de Projetos para Agências de Marketing Digital**. O objetivo do sistema é organizar e monitorar de forma inteligente o fluxo de demandas de criação de conteúdo (posts, vídeos, campanhas), automatizando a geração de planos de ação e a identificação de prazos e gargalos operacionais sem a necessidade de codificação tradicional.

---

## 🖥️ Protótipo
* **Link de acesso:** [Painel de Gestão no Airtable]([https://airtable.com](https://airtable.com/invite/l?inviteId=invdQTqUrGRJ3Fcvi&inviteToken=6a2e681d2236a0f372bc53cf7eded8d8f54b741e72382eb54d40eeb2b96cb23f&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts))
* **Funcionamento:** O painel recebe o nome da demanda, o responsável técnico e o status atual. O campo nativo de Inteligência Artificial (`Attachment Summary` / AI Prompt Field) cruza esses dados estruturados de forma autônoma e gera um resumo gerencial com o status em tempo real e o próximo passo urgente para o profissional.

> Coloque os arquivos de imagem ou PDF na pasta `/docs`.

---

## ⚙️ Plataforma Utilizada
* **Plataforma:** Airtable.
* **Justificativa da escolha:** O Airtable foi selecionado por unir a simplicidade de uma planilha visual com o poder de um banco de dados relacional e recursos integrados de IA generativa. A plataforma permitiu implementar regras complexas de negócios utilizando apenas linguagem natural no prompt, cumprindo o objetivo de agilidade e entrega rápida exigidos para um MVP.

---

## ✅ Vantagens Identificadas
Com base na vivência prática no laboratório, identifiquei as seguintes vantagens:
1. **Prototipagem rápida:** A estrutura básica da aplicação, modelagem de dados e ativação da IA foram configuradas de forma autônoma em menos de uma hora.
2. **Automação de processos repetitivos:** A IA substituiu a necessidade de checagem manual diária de prazos, gerando diagnósticos automáticos sob medida.
3. **Análise de Contexto Eficiente:** A IA provou ser capaz de interpretar cenários diferentes (demandas paradas vs. concluídas) e alterar suas recomendações dinamicamente.

---

## ⚠️ Limitações Encontradas
Durante o desenvolvimento do mini-projeto, mapeei as seguintes restrições técnicas da plataforma:
1. **Trava de Esquema Relacional:** A IA é estritamente dependente da existência prévia dos campos. Ao tentar rodar um prompt citando colunas inexistentes (como 'Prazo Final'), o sistema rejeita a execução e aponta erro de estrutura.
2. **Dependência de Dados Mínimos:** O ecossistema recusa o processamento e não gera respostas de forma preventiva se os campos obrigatórios (*Name*, *Status* e *Assignee*) estiverem completamente vazios.
3. **Risco de lock-in tecnológico:** A lógica interna dos prompts de inteligência artificial e as automações configuradas ficam presas ao Airtable, não sendo possível exportá-las diretamente para código bruto caso o sistema mude no futuro.

---

## 📚 Reflexão Crítica
Para contornar as limitações de espaço visual das linhas do Airtable, utilizei engenharia de prompt focada em concisão, instruindo a IA a gerar respostas diretas de no máximo duas frases. 

Diante dos erros de esquema encontrados nos primeiros testes (tabela vazia e colunas faltantes), a experiência prática provou a necessidade de uma governança rígida de dados: uma IA no-code só é eficiente se a estrutura de colunas que a alimenta estiver perfeitamente saneada e padronizada. Concluí que, para validação ágil de mercado (MVP), o Airtable entrega alta performance, mas exige planejamento prévio do banco de dados antes da escrita do prompt.

---

## 👥 Colaboração
Trabalho realizado de forma **individual**. Gerenciei de forma integrada e autônoma todas as etapas do ciclo de desenvolvimento no laboratório: desde a modelagem dos tipos de campos, testes de tratamento de dados nulos, engenharia de prompt e validação com os registros de teste.

---

## 🧪 Validação dos Testes Práticos (Resultados do Sistema)
O funcionamento do protótipo foi validado com sucesso através de três cenários distintos preenchidos na tabela:

1. **Item Pendente (*Todo*):** 
   * *Entrada:* "Criação de Post de Carrossel - Dicas de Inverno"
   * *Retorno da IA:* "Demanda parada, ainda não iniciada. Responsável: Iniciar a produção do carrossel hoje."
2. **Item em Execução (*In progress*):** 
   * *Entrada:* "Edição de Vídeo Reels - Bastidores da Agência"
   * *Retorno da IA:* "Demanda em andamento. Responsável: Finalizar edição e submeter para aprovação imediata."
3. **Item Concluído (*Done*):** 
   * *Entrada:* "Identidade Visual - Cliente Hamburgueria"
   * *Retorno da IA:* "Demanda concluída. Responsável: Enviar entregáveis ao cliente e fechar o job."

---

## 📝 Registro da Aula
* **Data:** 11/05/2026
* **Atividade:** Discussão crítica + mini-projeto de aplicação
* **Local:** Laboratório de informática / Quadro branco
* **Professor(a):** Kadidja Valéria

---

## 🚀 Próximos Passos
* **Melhorias do protótipo:** Integrar a tabela do Airtable ao Slack ou WhatsApp através de ferramentas como Make ou Zapier, fazendo com que os alertas gerados pela IA sejam disparados como notificações push direto no bolso do responsável.
* **Evoluções para o Projeto Final:** Expandir o banco de dados criando tabelas relacionadas (múltiplas abas) para gerenciar o controle financeiro de custos por cliente e horas trabalhadas (*timesheet*) por demanda.

