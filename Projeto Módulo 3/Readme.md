# Projeto Módulo 3 – Low Code/No Code/Vibecode

## 📌 Desafio Escolhido

**Gerenciador de Clientes** para uma empresa de Empréstimo Consignado

---

## 🖥️ Protótipo

[![Protótipo Funcional](https://img.shields.io/badge/protótipo-funcional-success)](https://airtable.com/invite/l?inviteId=invXRtQxD6jsvj63B&inviteToken=86551a913a5f7e139889d50e53f14f55120077c82f93db502429804c589b58fa&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts)

### Como Funciona

O sistema permite que o usuário (vendedor) cadastre clientes de forma simples e intuitiva, preenchendo informações essenciais:
- **Nome do Cliente**
- **Email**
- **CPF**
- **Número de Telefone**
- **Vínculo** (tipo de relação com a empresa)
- **Tipo de Operação** (tipo de empréstimo ou serviço)
- **Nome do Vendedor** (para controle de responsabilidade)

Após o cadastro, os dados são organizados em uma base de dados relacional e podem ser pesquisados, filtrados e atualizados rapidamente através da interface intuitiva do Airtable.

---

## ⚙️ Plataforma Utilizada

### Airtable

**Justificativa da Escolha:**

O Airtable foi selecionado por unir o poder de um banco de dados relacional à flexibilidade de uma interface no-code personalizada. Os principais motivos foram:

- **Desenvolvimento Ultra-Rápido**: Permite criar um gerenciador de clientes sem necessidade de codificar um backend do zero
- **Interface Designer Poderosa**: Possibilita criar uma tela minimalista e focada na experiência do usuário
- **Autonomia do Usuário**: Oferece total liberdade para o vendedor gerenciar e criar suas próprias listas de oportunidades de forma dinâmica
- **Segurança e Organização**: Mantém os dados seguros, organizados e prontos para automações que melhoram a qualidade de vida operacional

---

## ✅ Vantagens Identificadas

1. **Desenvolvimento Rápido**
   - Foi possível criar o sistema em pouco tempo, sem necessidade de programação avançada
   - Redução significativa no time-to-market

2. **Interface Simples e Intuitiva**
   - A plataforma permitiu organizar as informações de forma visual e fácil de entender
   - Curva de aprendizado mínima para novos usuários

3. **Facilidade de Gerenciamento**
   - Sistema permite cadastrar, pesquisar e visualizar clientes rapidamente
   - Campos de pesquisa dinâmicos facilitam localização de registros
   - Operações CRUD (Create, Read, Update, Delete) simplificadas

---

## ⚠️ Limitações Encontradas

1. **Customização Limitada**
   - Algumas alterações visuais e funcionalidades avançadas dependem das limitações técnicas da plataforma
   - Restrições no styling e comportamentos personalizados

2. **Dependência da Plataforma**
   - O sistema funciona exclusivamente dentro do Airtable, criando dependência da ferramenta
   - Migração de dados pode ser complexa em caso de mudança de plataforma

3. **Restrições do Plano Gratuito**
   - Algumas automações e funcionalidades avançadas possuem limitações
   - Controle de acesso baseado em permissões é restrito nos planos mais básicos

---

## 📚 Reflexão Crítica

### Desafios Enfrentados e Soluções

Durante o desenvolvimento, enfrentei limitações significativas que exigiram criatividade:

**Problema 1: IA do Airtable Limitada**
- O assistente de IA do Airtable falhava ao gerar tabelas conectadas em um único comando
- **Solução Aplicada**: Estruturei o banco relacional manualmente e utilizei a IA apenas para otimizar o layout visual

**Problema 2: Controle de Acesso por Usuário (Ainda em Desenvolvimento)**
- A dificuldade principal foi configurar o sistema para que cada usuário visualize apenas os clientes que ele mesmo cadastrou
- Restrições do plano gratuito e limitações técnicas da ferramenta impossibilitaram implementação completa
- **Mitigação Temporária**: 
  - Campo 'Nome do Vendedor' mantido visível para rastreabilidade
  - Barra de pesquisa rápida permite que cada operador localize facilmente seus próprios registros
  - Esta é uma melhoria prioritária para futuras versões

### Aprendizados

O projeto demonstrou que ferramentas no-code são excelentes para prototipagem rápida, mas apresentam trade-offs entre velocidade de desenvolvimento e controle granular de funcionalidades avançadas.

---

## 👥 Colaboração

O projeto foi desenvolvido **individualmente** (solo) com suporte externo limitado.

**Processo Colaborativo:**
- A única ajuda externa veio da equipe da empresa parceira, que forneceu recomendações de melhorias e casos de uso reais
- Essas recomendações foram incorporadas ao design do sistema, garantindo aderência aos requisitos do negócio

---

## 📝 Registro da Aula

| Item | Detalhes |
|------|----------|
| **Data** | 18/05/2026 |
| **Atividade** | Discussão crítica + mini-projeto de aplicação |
| **Local** | Laboratório de informática |
| **Professor(a)** | Kadidja Valéria |

---

## 🚀 Próximos Passos

### Melhorias Planejadas

1. **Implementar Controle de Acesso por Usuário**
   - Cada vendedor visualiza apenas seus próprios clientes
   - Gerentes e supervisores têm visibilidade total
   - Requer upgrade do plano ou migração para plataforma com mais controle granular

2. **Criar Listas de Futuras Oportunidades**
   - Pipeline de oportunidades para prospecção
   - Vinculação entre clientes e oportunidades

---

**Autor**: Arthur Coelho  
**Data de Atualização**: 18/05/2026

