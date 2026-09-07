# Roteamento de Redes Multi-Classe no Cisco Packet Tracer

## Resumo
Implementação de topologia de redes no Cisco Packet Tracer para conectar e rotear o tráfego de dados entre três sub-redes corporativas isoladas (Classes A, B e C) através de um roteador central Cisco 2911.

---

## 1. O que é este projeto?
Pense em três prédios vizinhos de uma empresa: o Financeiro (Rede A), o Comercial (Rede B) e a Operação (Rede C). Dentro de cada prédio, as pessoas conversam diretamente através de um switch local. Porém, para trocar mensagens entre prédios diferentes, elas precisam passar pela portaria central (o roteador). O roteador confere o endereço de destino e encaminha a mensagem pela porta certa para o prédio correspondente.

---

## 2. Objetivo e Valor para o Negócio
- **Problema Enfrentado:** Necessidade de segmentar setores corporativos em faixas de IP distintas por organização e controle de tráfego, mantendo a comunicação liberada e segura entre eles.
- **Solução Aplicada:** Criação de uma topologia com 3 switches Cisco 2960 conectados a 1 roteador Cisco 2911, configurando endereçamento IPv4 estático e gateways dedicados para cada classe de rede.
- **Impacto Prático:** Isolamento de domínios de broadcast (evitando lentidão local), contenção de falhas e garantia de roteamento eficiente entre departamentos.

---

## 3. Tecnologias e Competências Praticadas
- **Ambiente e Ferramentas:** Cisco Packet Tracer, Roteador Cisco 2911, Switches Cisco 2960-24TT, Hosts Finais (PC-PT).
- **Técnicas e Metodologias:** Endereçamento IPv4 Classful (Classes A, B e C), parametrização de gateways, interconexão física via cabo direto e diagnóstico de tráfego via ICMP.
- **Competências Profissionais Evidenciadas:** Arquitetura de redes locais (LAN), configuração CLI no Cisco IOS e resolução metódica de incidentes de conectividade.

---

## Topologia e Arquitetura de Rede

<img width="1919" height="627" alt="image" src="https://github.com/user-attachments/assets/c87e1dee-1aa0-4135-86e2-e418ee63704c" />


A rede está dividida em 3 zonas/segmentos distintos:

| Segmento / Classe | Endereço de Rede | Gateway Padrão | Máscara de Rede | Função Simulada |
| :--- | :--- | :--- | :--- | :--- |
| **Rede A (Classe A)** | `10.0.0.0/8` | `10.0.0.1` | `255.0.0.0` | Zona Corporativa / Servidores |
| **Rede B (Classe B)** | `172.16.0.0/16` | `172.16.0.1` | `255.240.0.0` | Estações de Trabalho / Visitantes |
| **Rede C (Classe C)** | `192.168.1.0/24` | `192.168.1.1` | `255.255.255.0` | Dispositivos Críticos / Admins |

---
