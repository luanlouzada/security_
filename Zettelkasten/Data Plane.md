---
title: PN-202511032223-Data Plane
tags:
  - security
  - se01
  - dataplane
created: 2025-11-17
modified: 2025-11-17
status: "#completed"
---

# Data Plane

## Resumo

O **Data Plane** (Plano de Dados), também conhecido como *forwarding plane*, é a parte "operacional" de um sistema de rede. É a força de trabalho que executa as tarefas de encaminhamento, filtragem e processamento de pacotes de dados.

Ele não toma decisões; em vez disso, ele segue as regras e tabelas de encaminhamento que foram criadas e enviadas pelo [[Control Plane]]. Sua principal função é mover o tráfego da entrada para a saída correta da forma mais rápida e eficiente possível.

- **[[Control Plane]]**: Pensa e decide.
- **Data Plane**: Executa as ordens.

###### Elementos de Interação e Controle de Fluxo

[[Subject-System|Subject/System]]
[[Policy Enforcement Point]]

---

### Exemplo Prático: Um Roteador de Rede

Continuando com o exemplo do roteador:

1. **[[Control Plane]]**:
2. - Calcula a melhor rota e cria a **tabela de roteamento**.
3. **Data Plane**:

   - É o hardware especializado (como ASICs) que lida diretamente com os pacotes.
   - Quando um pacote chega a uma porta do roteador, o Data Plane olha o endereço de destino do pacote.
   - Ele faz uma consulta ultrarrápida na tabela de roteamento (fornecida pelo Control Plane) para ver para qual porta de saída o pacote deve ir.
   - Finalmente, ele encaminha o pacote para essa porta de saída. Todo esse processo acontece em microssegundos, sem precisar consultar o "cérebro" (Control Plane) para cada pacote individual.

**Analogia Simples:**

- **[[Control Plane]]** é o estrategista que desenha o mapa da batalha.
- **Data Plane** é o soldado na linha de frente que usa o mapa para ir do ponto A ao ponto B, sem questionar e o mais rápido possível.
