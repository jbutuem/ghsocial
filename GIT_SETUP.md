# 🚀 Como subir esse repo

Esse repo já está inicializado com Git, primeiro commit feito e tag `v.2026.07-rev4` criada.
Falta só conectar com um remote (GitHub, GitLab, Bitbucket, etc) e dar push.

## Opção 1 · GitHub

### A) Criar repo via web
1. Vai em https://github.com/new
2. Nome sugerido: `gamerhut-social-playbook`
3. **Marcar como Privado** (é IP da Gamer Hut)
4. **NÃO inicializar** com README/license/gitignore — já tem aqui
5. Criar

### B) Conectar e dar push
```bash
cd gamerhut-social-playbook

# Adicionar remote
git remote add origin git@github.com:SEU-USER/gamerhut-social-playbook.git
# OU via HTTPS:
git remote add origin https://github.com/SEU-USER/gamerhut-social-playbook.git

# Push do main
git push -u origin main

# Push das tags (release v.2026.07-rev4)
git push origin --tags
```

---

## Opção 2 · GitLab

```bash
git remote add origin git@gitlab.com:SEU-USER/gamerhut-social-playbook.git
git push -u origin main
git push origin --tags
```

---

## Opção 3 · Bitbucket

```bash
git remote add origin git@bitbucket.org:SEU-USER/gamerhut-social-playbook.git
git push -u origin main
git push origin --tags
```

---

## ✅ Verificar que subiu

```bash
git remote -v
git log --oneline --decorate
git tag -l
```

Deve aparecer:
- `origin` no remote
- 1 commit `feat: estrutura inicial...`
- Tag `v.2026.07-rev4`

---

## 🔧 Configurar Netlify pra deploy automático

Já tem `netlify.toml` configurado e workflow `.github/workflows/deploy.yml` que valida estrutura.

1. Vai em https://app.netlify.com
2. **Add new site** → **Import from Git**
3. Conecta com GitHub e seleciona `gamerhut-social-playbook`
4. **Build command**: deixa vazio
5. **Publish directory**: `.` (raiz)
6. Deploy

URL fica tipo: `https://gamerhut-social-playbook.netlify.app`

(Pode adicionar domínio próprio em Domain settings depois)

### Pra ativar deploy via GitHub Actions

Em GitHub → Settings → Secrets → Actions, adicionar:
- `NETLIFY_AUTH_TOKEN` (pega em Netlify → User settings → Applications → Personal access tokens)
- `NETLIFY_SITE_ID` (pega em Netlify → Site settings → General)

Aí cada push em `main` ativa validação automática + deploy.

---

## 📦 Workflow de release zip

Já tem `.github/workflows/release.yml` que **gera zip automaticamente** quando você cria uma nova tag:

```bash
# Quando subir uma nova versão
git tag -a v.2026.07-rev5 -m "rev5 · ajustes pontuais"
git push origin v.2026.07-rev5

# GitHub Actions vai gerar gamerhut-social-playbook-v.2026.07-rev5.zip
# E criar uma Release com release notes automáticas
```

---

## 🎯 Branch strategy sugerida

- `main` — versão estável publicada
- `dev` — em desenvolvimento ativo
- `feat/XXX` — features novas
- `fix/XXX` — correções

```bash
# Começar nova feature
git checkout -b feat/agosto-2026

# Quando terminar
git checkout main
git merge feat/agosto-2026
git tag -a v.2026.08 -m "Agenda agosto 2026"
git push origin main --tags
```
