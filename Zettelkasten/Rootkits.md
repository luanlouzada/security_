---
title: PN-202511161906-Rootkits
tags:
  - security
  - se06
  - rootkits
created: 2025-11-17
modified: 2025-11-17
status: "#completed"
---

# Rootkits

## Resumo

É um tipo específico de software projetado para obter controle de nível administrativo sobre um determinado sistema de computador sem ser detectado

Ele tenta escalar privilégios desde do RING 3 até o 0

Dá acesso ao Ring 1(administrador) ou zero(Kernel Mode), permite que o sistema controle o acesso a itens como drivers de dispositivos, placa de som, monitor etc

Difícil detecção por anti-vírus ou anti-malware

###### Técnica usada pelos rootkits

[[DLL Injection]]

## Flashcards

O que é um Rootkit?
?
É um tipo específico de software projetado para obter controle de nível administrativo sobre um determinado sistema de computador sem ser detectado
