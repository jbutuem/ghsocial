# Changelog · GAMER HUT Social Media Playbook

Todas as mudanças notáveis nesse projeto serão documentadas aqui.
Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/).

## [v.2026.09-L2] · 2026-05-08 · alinhamento total ao guia oficial

### Mudou (correções críticas ao L1)
- **Tom de voz: 5 → 3 pilares**. O guia oficial v.2026.09 define 3 pilares de TOM (Acessível · Transparente · Instigante) + 4 pilares da ESSÊNCIA (Acessível · Transparente · Instigante · Confiável). L1 tinha colocado 5 pilares baseado no doc anterior — corrigido.
- **"Bora" BANIDO como CTA** (regra de ouro 6). Substituído globalmente por: "Garanta o seu" · "Pré-venda liberada" · "Link na Bio" · "Novidade no estoque".
- **"NF" agora é implícito** (regra de ouro 5). Removido de copy de marketing — fica só em selo institucional. "Original. Lacrado. Com NF." virou "Original e lacrado".
- **Gen Z: 16-29 → 18-29**. Faixa etária atualizada conforme o guia.

### Adicionou
- **Manifesto curto** ("Somos os experts. Criado por quem joga, coleciona e respeita o jogo...") em destaque no Stage 01.
- **4 pilares da ESSÊNCIA** (A·Acessível · B·Transparente · C·Instigante · D·Confiável) no Stage 01.
- **Vocabulário oficial USE × NUNCA** em tabela visual no Stage 01.
- **10 regras de ouro inegociáveis** numeradas e destacadas no Stage 01.
- **Cheat Sheet USE × EVITE por situação** (6 situações: abertura, procedência, CTA, comunidade, pós-venda, limites) no Stage 01.
- **4 casos de uso reais** com exemplos prontos (GTA VI · MGS Δ · DM Pokémon · AC Black Flag) no Stage 13 Anatomia.
- **Hooks aprovados** específicos por geração no Stage 02 Audiências (Symphony of the Night pra Gen X · Black Flag pra Mill · Mario Kart pra Gen Z).
- **Stage 20 NOVO · Checklist Final**: 12 perguntas interativas com checkboxes antes de apertar publicar.
- **Stage 21 · Staff Roll**: ganhou manifesto curto + "Powered by TGT" + "agência além do marketing" + atualização de versão.
- **Chips geracionais** aplicados em: 6 pipeline cards · 4 lançamentos · 4 datas comemorativas · 5 arcos de stories · 6 reels · 4 carrosseis (29 chips no total).
- Mensagem-âncora "MÍDIA FÍSICA NEVER DIES" reforçada em destaque visual no Stage 01 e no Staff Roll.

### Removeu
- Repetição de "NF" em copies de marketing (mantida só em selos institucionais e quando é regra explícita).
- Uso de "Bora" como CTA em todos os copies do calendário, anatomias, reels e launches.
- 5 pilares de tom de voz (substituído pelo modelo oficial 3 pilares de tom + 4 pilares de essência).

### Compliance final
- ✓ 0 ocorrências de "hut" sozinho
- ✓ 0 ocorrências de "Bora" como CTA real
- ✓ 0 ocorrências de "NF" como bandeira em copy de marketing
- ✓ 0 ocorrências de "tua/teu" em copies de marketing (mantido só em meta-referência à regra)
- ✓ Sections balanceadas 22/22
- ✓ Divs balanceadas 1711/1711
- ✓ Squad 9 publishers completo (Nintendo · Sony PS · Microsoft · Capcom · Rockstar · Konami · SEGA · Bandai Namco · Ubisoft)
- ✓ "Powered by TGT · A Agência Além do Marketing" no rodapé

### Próximo
- **L3 / L4 (opcional)**: consolidar 3 stages de Feed em 1, adicionar Hashtag Bank seg. por geração, KPIs matriz por geração×canal.

---

## [v.2026.09-L1] · 2026-05-08

### Adicionou
- **Stage 02 NOVO · Audiências geracionais**: 3 cards lado a lado (Gen X · Millennials · Gen Z) com hooks, tom dominante, formato preferido, mecânica de venda e % que paga preço cheio.
- **Stage 03 NOVO · Canal × Geração**: matriz cruzada de 10 canais × 3 audiências (Google, YouTube longo/Shorts, Instagram, TikTok, Twitch, Discord, E-mail, WhatsApp). Sistema ★★★ ★★ ★ —.
- **Tom de voz expandido** · 3 → 5 pilares: Descontraído + Próximo + Transparente + Instigante + Profissional sem perder personalidade gamer (no Stage 01).
- **5 Sentimentos como bússola**: Segurança · Exclusividade · Paixão · Inovação · Credibilidade (no Stage 01).
- **SQUAD 9 publishers** como bloco de credibilidade explícito (Nintendo · Sony PlayStation · Microsoft · Capcom · Rockstar · Konami · SEGA · Bandai Namco · Ubisoft).
- **Stage 04 · Meta Split Geracional**: KPIs desagregados por audiência. 45% esforço Gen Z (buzz) · 35% Mill (ticket médio) · 20% Gen X (ticket alto). Receita esperada concentrada 60-70% em Mill + Gen X.
- **Hero Stage 00**: stat "03 audiências · 1 plano".
- **CSS novo**: gen-chip, audience-card, channel-matrix, tom-grid, sentimento-pill, squad-block, meta-split-grid, key-read.

### Mudou
- **Stages renumerados**: 02-18 viraram 04-20 pra abrir espaço pros 2 novos. Total temporário: 21 stages (volta pra 19 no L3 quando consolidar os 3 feeds em 1).
- **Briefing (Stage 01)** reescrito: passa de "3 pilares de tom" pra "5 pilares + 5 sentimentos + regra de ouro multi-geracional + SQUAD 9".

### Próximos lotes
- **L2**: Pilares · Pipeline com chips · Lançamentos segmentados · Datas segmentadas · Calendário com chips
- **L3**: Feeds consolidado · Anatomia 3-chips · Stories · Reels · Carrosseis tagueados
- **L4**: Hashtag bank segmentado · KPIs matriz · Agenda · Staff Roll v.2026.09

---

## [v.2026.07-rev5] · 2026-05-08

### Removeu
- **Lock screen com senha** — playbook agora abre direto, sem gate de acesso.
- HTML do bloco lock-screen (id `lockScreen` com input/btn/error/hint).
- 12 regras CSS `.lock-*` (lock-screen, lock-card, lock-logo, lock-title, lock-tag, lock-input, lock-btn, lock-error, lock-hint).
- Bloco JS de "Lock Screen" (constante `PASSWORD`, função `tryUnlock`, check em `sessionStorage`).
- Animation `@keyframes lockPulse` (dead code).
- Função `playStartFanfare()` (era chamada apenas no unlock).

### Por quê
Solicitação do cliente — preferência por acesso aberto, facilita compartilhamento interno e externo sem fricção.

---

## [v.2026.07-rev4] · 2026-05-08

### Mudou
- **Stories ganharam cor temática**: 46 cards do Stage 12 foram coloridos por tipo de tag (▶ DROP laranja, ▶ NERD DAY roxo, ▶ CUPOM vermelho, ▶ ENQUETE roxo profundo, ▶ STOCK amarelo, ▶ REPOST cinza-azul, etc).
- Barra superior dos cards agora varia de cor seguindo o gradient do tipo.

### Por quê
Feedback do cliente: Stories estavam "vazios de imagem" (chapados, monocromáticos). A correção dá hierarquia visual e legibilidade temporal aos arcos narrativos.

---

## [v.2026.07-rev3] · 2026-05-07

### Adicionou
- CSS faltante completo pros componentes v2: anatomy-thumb, reel-mock, slides v2, ig-tile-tag, story-strip, arc-header.

### Mudou
- Stories cards: aspect-ratio mudou de `9/16` para `3/4` (proporção mais usável).
- Footer dos stories: fonte de `.5rem` para `.58rem` (legibilidade).

### Removeu
- 255 linhas de CSS v1 morto que duplicava classes do v2 (.slide, .slides-row, .reel-card, .carrossel-card).

### Consertou
- Conflito entre `.slide` v1 (com `width:230px` fixo) e `.slide` v2 (em grid responsivo).
- Conteúdo zumbi do v1 nos stages 12, 13 e 14 (700 linhas removidas cirurgicamente).

---

## [v.2026.07-rev2] · 2026-05-07

### Mudou
- Eliminado uso isolado de "hut" — sempre "Gamer Hut" ou "GH".
- Tiles de feed reforçados com ornamentos (patterns, badges arcade, deco corners).
- Reels Mães + AC Black Flag receberam fundos com camadas.
- Anatomias Pipeline/Mães/Nerd/DQ40 ganharam pattern + ornamentos arcade.

### Adicionou
- Imagens reais de jogos como background dim em tiles que estavam só com gradient.

---

## [v.2026.07] · 2026-05-07

### Adicionou
- **Stage 04 — Pipeline Pré-Vendas**: 6 cards com 007 First Light · TGYH · Tides of Tomorrow · Mouse P.I. · AC Black Flag Resynced · MGS Master Collection Vol.2.
- **Stage 05 — Lançamentos do Período**: 4 launch-rows detalhados (007 27/05, AC 9/07, Mouse 10/07, MGS 27/08).
- **Stage 06 — Datas Comemorativas**: Mães (10/05), Nerd Day (25/05), DQ 40 (27/05), KI 40 (18/06).
- **Stage 17 — Agenda Longa Q3-Q4**: MGS Vol.2 launch (ago), BGS (out 9-12), CCXP (dez 3-6).
- 17 imagens novas das pré-vendas (007, TGYH, TOT, AC, Mouse, MGS).

### Mudou
- Janela do plano: de 45 dias (16 mai → 30 jun) → **66 dias** (9 mai → 13 jul) — 9 semanas + 4 dias.
- Estrutura: 16 → **19 stages**.
- Tom de voz alinhado ao Brandbook v.2026.07: paleta 60-30-10 (Black 60% + Orange 30%), tags SQUAD removidas, "tua/teu" → "sua/seu", NF removido de copy de marketing.

---

## [v.2026.05] · 2026-05-07

### Versão inicial
- 16 stages cobrindo briefing, north star, pilares, calendário 45 dias, 3 feeds mockup, 6 anatomias, 4 arcos stories, 5 reels, 4 carrosseis, 4 ativações épicas, hashtag bank, KPIs.
- Easter eggs: senha gamerhut2026, Konami code, BGM chiptune Web Audio.
