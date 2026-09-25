---
title: "Canal YouTube @brncesarms: Engenharia de Redes & Caderno de Bancada"
date_created: 2026-09-24
last_modified: 2026-09-25
author: "Bruno César"
privacy: public
tags:
  - publico
  - canal-youtube
  - mikrotik
  - routeros7
  - telecom
  - networking
  - audiovisual
  - indice
---

# 🌐 Canal YouTube @brncesarms: Engenharia de Redes & Caderno de Bancada

[![YouTube](https://img.shields.io/badge/YouTube-%40brncesarms-FF0000?logo=youtube&logoColor=white)](https://youtube.com/@brncesarms)
[![RouterOS](https://img.shields.io/badge/MikroTik-RouterOS%20v7-1F4F7C)](https://mikrotik.com)
[![OBS Studio](https://img.shields.io/badge/Captura-OBS%20Studio%20(4K)-302E31?logo=obsstudio&logoColor=white)](https://obsproject.com)
[![DaVinci Resolve](https://img.shields.io/badge/Edição-DaVinci%20Resolve-0E1017)](https://www.blackmagicdesign.com)
[![Obsidian](https://img.shields.io/badge/Obsidian-Zettelkasten-7C3AED?logo=obsidian&logoColor=white)](https://obsidian.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

Repositório público oficial do canal [`@brncesarms`](https://youtube.com/@brncesarms), mantido por **Bruno César**.

Atua como o **Caderno de Bancada Aberto** e centro de documentação técnica para alunos, inscritos e profissionais de telecomunicação, contendo roteiros atômicos, topologias visuais, diagramas em blocos, matrizes de cálculo e comandos práticos das aulas.

---

## 🏛️ Pipeline de Engenharia de Conteúdo & Produção Audiovisual

Da idealização da topologia até a entrega do vídeo final em 4K UltraHD:

```mermaid
flowchart TD
    subgraph Pre ["📝 1. Engenharia & Roteirização"]
        Idea["Definição do Tema & Dor de Mercado"]
        Vault["Caderno de Bancada no Obsidian<br/>(Diagramas Mermaid + Comandos RouterOS v7)"]
        Lab["Montagem de Bancada Virtual<br/>(PNETLab / CHR em Cluster)"]
        Idea --> Vault --> Lab
    end

    subgraph Studio ["🎙️ 2. Estúdio & Captação"]
        Alien["Workstation ALIENWARE (RTX 5060)<br/>Omarchy Linux / Hyprland"]
        OBS["OBS Studio 30+ (Wayland / PipeWire)"]
        NVENC["Encoder NVENC 4K @ 60 FPS<br/>CQP 18 / Áudio RNNoise"]
        Alien --> OBS --> NVENC
    end

    subgraph Post ["✂️ 3. Pós-Produção"]
        DaVinci["DaVinci Resolve Studio (Linux)"]
        EBUR128["Normalização EBU R128 (-14 LUFS)"]
        Master["Master H.265 4K UltraHD"]
        DaVinci --> EBUR128 --> Master
    end

    subgraph Delivery ["🚀 4. Entrega & Vitrine Pública"]
        YouTube["🎬 YouTube (@brncesarms)<br/>Aulas Gratuitas com Alta Retenção"]
        GitHub["💼 GitHub (brncesarms/canal-youtube)<br/>Apostila Aberta para a Comunidade"]
        YouTube <--> GitHub
    end

    Lab --> Studio
    NVENC --> Post
    Master --> Delivery
```

---

## 📖 Catálogo de Notas & Materiais Complementares

### ⚙️ Engenharia de Estúdio & Diretrizes
- 🎬 [Pipeline de Produção Audiovisual & Estúdio](./00_pipeline_producao_audiovisual.md) — Configurações de OBS, PipeWire, filtros de áudio e encoder NVENC.
- 📚 [Diretrizes Editoriais & Framework de Roteirização](./04_diretrizes_editoriais_e_roteirizacao.md) — Metodologia didática dos 4 blocos de retenção.

### 🔷 Curso MikroTik Básico 2026: Do Zero ao BGP
| Aula | Assunto | Roteiro Completo & Caderno de Bancada | Destaques Técnicos |
|:---:|:---|:---|:---|
| **01** | Ecossistema Moderno | [01 - O Novo Ecossistema MikroTik em 2026](./01_introducao_ecossistema_mikrotik_2026.md) | Transição MIPSBE para ARM64, Kernel 5.6+, L3HW Offloading e CHR |
| **02** | IPv4 & Subnetting | [02 - Endereçamento IPv4 & Notação CIDR sem Decoreba](./02_enderecamento_ipv4_e_mascaras_cidr.md) | Método mental das potências de 2, RFC 1918, CGNAT RFC 6598 e Enlace `/31` |
| **03** | Arquitetura TCP/IP | [03 - Arquitetura TCP/IP, Three-Way Handshake & Tabela ARP](./03_arquitetura_tcp_ip_handshake_e_arp.md) | Encapsulamento, Connection Tracking no RouterOS v7, portas e proteção `arp=reply-only` |

---

## 🛠️ Tecnologias & Ambiente de Bancada

- **Hardware Virtual:** MikroTik Cloud Hosted Router (CHR) no PNETLab / Proxmox VE.
- **Sistema Operacional de Roteamento:** MikroTik RouterOS v7.16+ (Kernel Linux 5.6+).
- **Gerenciamento:** Winbox 4 (Nativo Linux/macOS/Windows) & SSH com chaves Ed25519.
- **Estação de Trabalho:** Omarchy Linux (Hyprland / Tokyo Night).
- **Toolbox de Automação:** [`brncesarms/scripts`](https://github.com/brncesarms/scripts).

---

## 🔗 Repositórios Relacionados no Ecossistema

- 🌐 [redes](https://github.com/brncesarms/redes) — Topologias corporativas, OSPF, VPN Tailscale e Firewall Stateful.
- 🐧 [linux](https://github.com/brncesarms/linux) — Transcodificação FFmpeg com NVENC, SO e virtualização KVM.
- 🪟 [windows](https://github.com/brncesarms/windows) — Configurações de estações de trabalho e OpenSSH.
- 🤖 [ia](https://github.com/brncesarms/ia) — Inferência local e RAG com sqlite-vec.
- 🧰 [scripts](https://github.com/brncesarms/scripts) — Toolbox multiplataforma determinística.

---

## 📜 Licença

Distribuído sob a licença **MIT**. Consulte `LICENSE` para mais detalhes.  
Criado e mantido por **Bruno César** ([@brncesarms](https://github.com/brncesarms)).
