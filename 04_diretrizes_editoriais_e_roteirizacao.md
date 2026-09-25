---
title: "Diretrizes Editoriais, Framework de Roteirização & Padrão Didático"
date_created: 2026-09-25
last_modified: 2026-09-25
author: "Bruno César"
privacy: public
tags:
  - publico
  - canal-youtube
  - diretrizes
  - roteirizacao
  - didatica
  - mikrotik
---

# 📚 Diretrizes Editoriais & Framework de Roteirização

> [!info] Metodologia didática e framework de estruturação de aulas técnicas para o canal [@brncesarms](https://youtube.com/@brncesarms), focada em alta retenção, clareza conceitual com diagramas visuais e laboratórios 100% reproduzíveis.

---

## 🧭 1. Framework dos 4 Blocos de Retenção

Cada aula técnica do canal é desenhada seguindo a estrutura de 4 blocos progressivos:

```mermaid
flowchart LR
    A["🪝 Bloco 1: O Gancho<br/>(0 a 30 seg)<br/>A dor do mercado e o que será construído"] --> B["🧠 Bloco 2: Fundamentação Visual<br/>(1 a 3 min)<br/>Diagramas Mermaid / Mapas Mentais"]
    B --> C["⚡ Bloco 3: Laboratório Prático<br/>(4 a 12 min)<br/>Comandos CLI e Winbox 4 sem cortes"]
    C --> D["🎯 Bloco 4: Recap & Próximo Passo<br/>(Último minuto)<br/>Resumo em 3 pontos e CTA"]
```

### Detalhamento dos Blocos:
1. **O Gancho (Hook Imediato):** Sem vinhetas longas ou saudações demoradas. Apresentação imediata do problema real enfrentado por provedores ou engenheiros de infraestrutura e a demonstração do resultado final funcionando.
2. **Fundamentação Visual (Conceito):** O conceito teórico é explicado com diagramas em blocos (Mermaid), tabelas comparativas e analogias diretas de engenharia, eliminando decoreba teórica.
3. **Hands-on de Bancada (Prática Real):** Execução passo a passo no terminal RouterOS v7 ou Winbox 4. Comandos documentados no caderno de bancada no Obsidian.
4. **Recapitulativo & Próximo Passo:** Síntese do aprendizado e ponte lógica para o próximo episódio da série.

---

## 🛠️ 2. Padrões Inegociáveis de Conteúdo (Zero Gambiarras)

- **Tecnologia Atualizada (2026):** Foco estrito em **RouterOS v7**, arquiteturas modernas ARM64/x86_64, Winbox 4 multiplataforma e túneis WireGuard/Tailscale.
- **Transparência de Cenário:** Toda topologia de laboratório deve ser clara quanto ao endereçamento IP, interfaces e restrições de ambiente virtual.
- **Caderno de Bancada Aberto:** Os inscritos têm acesso aos exatos scripts e anotações exibidos na tela através do repositório público `canal-youtube` no GitHub.

---

## 🔗 Notas Relacionadas
- [Pipeline de Produção Audiovisual & Estúdio](00_pipeline_producao_audiovisual.md) — Infraestrutura técnica de hardware e software.
- [Aula 01: O Novo Ecossistema MikroTik em 2026](01_introducao_ecossistema_mikrotik_2026.md) — Aplicação prática do framework didático.
- [Aula 02: Endereçamento IPv4 e Máscaras CIDR](02_enderecamento_ipv4_e_mascaras_cidr.md) — Guia visual de cálculo de blocos.
- [Guia Principal do Canal YouTube](README.md) — Índice geral do canal e materiais complementares.
