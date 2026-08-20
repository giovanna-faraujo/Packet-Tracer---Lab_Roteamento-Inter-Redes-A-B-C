# Laboratório de Roteamento Inter-VLANs e Arquitetura de Redes (Cisco Packet Tracer)

## Visão Geral
Este laboratório simula a infraestrutura de uma rede corporativa segmentada em sub-redes (Classes A, B e C), interconectadas por um roteador central. O objetivo é demonstrar conceitos fundamentais de arquitetura de redes, endereçamento IP e aplicação de políticas de segurança e controle de acesso para perfis Júnior de Cybersecurity/SOC.

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
