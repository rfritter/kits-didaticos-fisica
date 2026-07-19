# 🚀 Como subir este repositório para o GitHub

## Opção A — Criar o repo pelo site e depois enviar (recomendado)

1. No GitHub, clique em **New repository**
   - Nome: `kits-didaticos-fisica`
   - Descrição: *Kits didáticos de física de baixo custo (ESP32/Arduino + FreeCAD + Python)*
   - Público
   - **NÃO** marque "Add a README" (já temos um)

2. No seu PC, dentro da pasta do projeto, rode:

```bash
cd kits-didaticos-fisica

# Inicializa o repositório local
git init
git branch -M main

# Configura seu autor (se ainda não fez globalmente)
git config user.name "Renan Ritter"
git config user.email "seu-email@exemplo.com"

# Primeiro commit
git add .
git commit -m "chore: estrutura inicial do projeto de kits didáticos"

# Conecta ao repositório remoto (troque SEU-USUARIO)
git remote add origin https://github.com/SEU-USUARIO/kits-didaticos-fisica.git

# Envia
git push -u origin main
```

## Opção B — Usando o GitHub CLI (gh)

```bash
cd kits-didaticos-fisica
git init && git branch -M main
git add . && git commit -m "chore: estrutura inicial do projeto de kits didáticos"
gh repo create kits-didaticos-fisica --public --source=. --push
```

---

## 🔑 Lembrete de segurança

O `.gitignore` já bloqueia arquivos de credenciais (`.env`, `secrets.h`,
`wifi_credentials.h`, etc.). **Sempre** guarde senhas de Wi-Fi e tokens
nesses arquivos ignorados — nunca direto no firmware versionado.

Antes de cada push, um bom hábito:
```bash
git status          # confira o que será enviado
git diff --staged   # revise as mudanças
```

---

## 🏷️ Sugestão de fluxo de trabalho

- Uma **branch por kit/feature**: `git checkout -b kit-01-queda-livre`
- **Commits pequenos e descritivos** (padrão Conventional Commits):
  - `feat: firmware de leitura dos sensores IR`
  - `docs: roteiro pedagógico do kit de queda livre`
  - `fix: corrige debounce da barreira óptica`
- **Tags** para marcos: `git tag -a v0.1-queda-livre -m "Primeiro kit funcional"`
