---
title: PN-202511012207-Authorization
tags:
  - security
  - se01
  - authorization
created: '"2025-11-17"'
modified: '"2025-11-17"'
status: "#completed"
---

# Authorization

## Resumo

Autorização é o processo que determina quais ações um usuário ou sistema autenticado tem permissão para executar. **Responde à pergunta: "O que você pode fazer?".**

## Conceitos Relacionados

Existem diferentes modelos para implementar a autorização:

- [[Role-Based Access Control (RBAC)]]
- [[Rule-Based Access Control (RuBAC)]]
- [[Attribute-Based Access Control (ABAC)]]

## Flashcards

Qual modelo de autorização concede acesso com base em um conjunto de regras dinâmicas, como horário de acesso?  
?  
RuBAC (Rule-Based Access Control). A decisão é baseada se um conjunto de **condições (regras)** é satisfeito.

Qual modelo de autorização atribui permissões a "papéis" (roles) em vez de usuários individuais?  
?  
RBAC (Role-Based Access Control). A decisão é baseada em **quem** é o usuário (qual o seu papel).

Qual é o modelo de autorização mais granular, que toma decisões com base em atributos do usuário, recurso e ambiente?  
?  
ABAC (Attribute-Based Access Control). A decisão é baseada em uma **combinação de múltiplos atributos**.
