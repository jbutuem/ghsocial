# Contribuir · GAMER HUT Social Playbook

## Como editar

1. Clonar o repo:
   ```bash
   git clone <url-do-repo>
   cd gamerhut-social-playbook
   ```

2. Abrir `index.html` direto no navegador — não precisa de servidor.

3. Editar conteúdo. O HTML é single-file por design (CSS embutido + JS embutido + assets/ apartados).

## Estrutura

```
.
├── index.html              # arquivo principal (CSS + HTML + JS)
├── README.md               # documentação geral
├── CHANGELOG.md            # histórico de revisões
├── LICENSE                 # propriedade GAMER HUT
├── .gitignore
├── .editorconfig
├── netlify.toml            # config de deploy Netlify
└── assets/
    ├── logos/              # logos GAMER HUT (6 arquivos)
    └── games/              # keyarts dos jogos (35 arquivos)
```

## Convenções

- **Stages**: cada seção é um Stage numerado (00-18).
- **CSS**: classes prefixadas por componente (`pipeline-`, `launch-`, `anatomy-`, `reel-`, `story-`, `ig-tile-`).
- **Tom de voz**: alinhado ao Brandbook v.2026.07. Sempre "Gamer Hut" ou "GH" — nunca "hut" sozinho.
- **Palavras banidas**: pirata, réplica, cópia, console novo, usado, "imperdível!!!", urgência fake.

## Workflow

1. Criar branch a partir de `main`: `git checkout -b feat/nome-da-feature`
2. Fazer mudanças e testar abrindo `index.html`
3. Commit com mensagem clara: `feat(stage12): adiciona variação de cor por tag`
4. PR pra `main`

## Commits

Convenção [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/):

- `feat:` nova funcionalidade
- `fix:` correção de bug
- `style:` mudança visual sem afetar lógica
- `docs:` mudança em documentação
- `chore:` manutenção/build
- `refactor:` refatoração sem mudar comportamento

## Versionamento

Formato: `v.{ANO}.{MES}-rev{N}` (ex: `v.2026.07-rev4`)

- Major: nova quinzena/mês de plano editorial
- Rev: ajustes/polishing dentro da mesma temporada
