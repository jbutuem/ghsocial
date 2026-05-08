# Changelog · GAMER HUT Social Media Playbook

Todas as mudanças notáveis nesse projeto serão documentadas aqui.
Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/).

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
