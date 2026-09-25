# 📱 Guia de Gravação & Estratégia de Conteúdo para o Instagram (@brncesarms)

> **Objetivo:** Posicionar Bruno César como autoridade técnica em Engenharia de Redes, MikroTik RouterOS v7 e Infraestrutura de Alta Disponibilidade, atraindo clientes de consultoria, provedores de internet e networking profissional.

---

## 🎬 1. Roteiro Gravado para Reels / TikTok (Vídeo de 60 Segundos)

### 📐 Formato Técnico:
- **Resolução:** 1080x1920 (Vertical 9:16) ou gravação da tela cheia com zoom no decágono.
- **Software:** OBS Studio (com atalho para zoom suave na tela) ou gravação nativa.
- **Cenário:** Tela do PNetLab aberta no `lab02` (Dark Mode ativado) com a topologia decagonal centralizada, e uma janela de terminal / Winbox dividindo a tela.

---

### ⏱️ Timeline & Fala do Roteiro (Palavra por Palavra)

```text
[00:00 - 00:04] 🪝 O GANCHO (Hook Visual + Frase de Impacto)
(Visual: Câmera fechada na topologia em anel no PNetLab, mostrando os 10 MikroTiks e o banner @brncesarms).
Fala: "Você sabe o que acontece quando uma escavadeira rompe a fibra óptica principal de uma grande empresa ou provedor?"

[00:05 - 00:15] 💥 O PROBLEMA
(Visual: Zoom na tela mostrando os enlaces e a arquitetura).
Fala: "Se a rede foi desenhada em estrela ou sem redundância, cai tudo: sistemas, internet e faturamento. Mas quando a engenharia é bem feita, a rede sequer percebe!"

[00:16 - 00:35] ⚙️ A DEMONSTRAÇÃO PRÁTICA (Autoridade na Tela)
(Visual: Terminal MikroTik ou Winbox aberto. Bruno dá um ping ininterrupto: /ping 10.255.0.6 src=10.255.0.1. Em seguida, desativa a interface ether2 do MK-01: /interface disable ether2).
Fala: "Olha só: aqui no meu laboratório no Proxmox, eu montei um anel metropolitano com 10 roteadores MikroTik rodando RouterOS v7 com OSPF em anel fechado. Eu vou 'cortar' o cabo agora ao vivo..."
(Visual: Apenas 1 pacote perdido ou ZERO perda, e a rota contorna automaticamente os 9 roteadores pelo outro lado do anel).
Fala: "Viu isso? O OSPF convergiu em milissegundos e o tráfego contornou o anel pelo sentido oposto sem derrubar o cliente!"

[00:36 - 00:48] 🎯 A LIÇÃO TÉCNICA
(Visual: Mostra a tabela de rotas atualizada e o card com as especificações).
Fala: "Isso é arquitetura de resiliência N+1. É esse nível de confiabilidade e alta disponibilidade que protege a operação de qualquer negócio crítico."

[00:49 - 00:60] 🚀 CHAMADA PARA AÇÃO (CTA)
(Visual: Volta para a visão geral do laboratório com o banner @brncesarms em destaque).
Fala: "Se você quer aprender mais sobre redes de alta performance ou precisa de consultoria para blindar a infraestrutura da sua empresa, já me segue aqui no perfil @brncesarms e me manda um direct!"
```

---

## 📸 2. Estrutura de Carrossel Didático para o Feed (5 Slides)

### Slide 1: Capa (Visual Hipnótico)
- **Imagem:** Print nítido da topologia decagonal do PNetLab em Dark Mode com glow neon ciano.
- **Texto Principal:** *"Como um anel de 10 roteadores MikroTik garante ZERO parada em empresas e provedores."*
- **Assinatura:** `@brncesarms`

### Slide 2: O Desafio de Redes Monoponto
- **Gráfico:** Comparação entre rede linear/estrela vs. anel redundante.
- **Explicação:** *"O custo de 1 hora de internet ou ERP fora do ar em uma operação comercial supera em 10x o custo de desenhar redundância."*

### Slide 3: Por que o RouterOS v7 em Anel?
- **Tópicos:**
  - OSPFv2/v3 nativo com detecção BFD.
  - Enlaces `/30` ponto-a-ponto isolados para rápida propagação de LSA.
  - Loopbacks `/32` estáveis independentes do estado físico das interfaces.

### Slide 4: O Teste de Ruptura (Failover na Prática)
- **Imagem:** Print do terminal MikroTik mostrando a saída do `/routing ospf neighbor print` e a tabela de rotas antes e depois do link cair.
- **Destaque:** Tempo de convergência inferior a 1 segundo.

### Slide 5: Apresentação & Contato
- **Foto/Avatar do Bruno:**
- **Bio curta:** *"Bruno César | Engenheiro de Redes & Infraestrutura. Especialista em MikroTik, Proxmox e automação."*
- **CTA:** *"Gostou do conteúdo? Salve para consultar depois e compartilhe com seu time de T.I. Dúvidas ou projetos? Chame no direct!"*

---

## 🎙️ 3. Dicas de Ouro para a Gravação
1. **Áudio é 50% do vídeo:** Se gravar voz, use um microfone de lapela ou headset com filtro de ruído no OBS (Filtro *Supressão de Ruído - RNNoise*).
2. **Movimento suave de mouse:** Evite sacudir o cursor. Destaque os elementos da tela com calma.
3. **Música de fundo:** No Instagram Reels, use um áudio em alta (trending áudio) em volume bem baixinho (10% a 15%) por baixo da sua voz.
4. **Legendas automáticas:** Use o recurso de legendas automáticas do Instagram ou CapCut — a maioria das pessoas assiste aos primeiros segundos de vídeos sem som!
