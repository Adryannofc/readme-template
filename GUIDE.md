# 📖 Guia Completo — README de Perfil no GitHub

> Template criado por **Adryann Felix** — [github.com/Adryannofc](https://github.com/Adryannofc)  
> Qualquer dúvida, me manda mensagem no LinkedIn ou abre uma issue no repositório.

---

## 📌 Índice

1. [O que é o README de perfil?](#1-o-que-é-o-readme-de-perfil)
2. [Criando o repositório especial](#2-criando-o-repositório-especial)
3. [Subindo o template](#3-subindo-o-template)
4. [Substituindo os campos](#4-substituindo-os-campos)
5. [Personalizando as badges de skills](#5-personalizando-as-badges-de-skills)
6. [Configurando as estatísticas automáticas](#6-configurando-as-estatísticas-automáticas)
7. [Configurando a Snake de contribuições](#7-configurando-a-snake-de-contribuições)
8. [Dicas finais para se destacar](#8-dicas-finais-para-se-destacar)

---

## 1. O que é o README de perfil?

O GitHub tem um recurso pouco conhecido: se você criar um repositório com o **mesmo nome do seu usuário**, qualquer arquivo `README.md` dentro dele aparece diretamente na sua página principal.

É como um cartão de visitas público — qualquer recrutador ou dev que acessar `github.com/SEU_USERNAME` vai ver seu perfil personalizado antes de qualquer repositório.

> 💡 **Exemplo:** meu usuário é `Adryannofc`, então meu repositório especial se chama `Adryannofc`.

---

## 2. Criando o repositório especial

1. Acesse [github.com/new](https://github.com/new)
2. No campo **Repository name**, digite **exatamente** o seu nome de usuário do GitHub
3. Marque **Public**
4. Marque **Add a README file**
5. Clique em **Create repository**

O GitHub vai exibir uma mensagem: *"✨ You found a secret!"* — isso confirma que o repositório especial foi criado corretamente.

---

## 3. Subindo o template

### Opção A — Pelo navegador (mais fácil)

1. Acesse o repositório que você acabou de criar
2. Clique no arquivo `README.md`
3. Clique no ícone de lápis ✏️ para editar
4. Selecione todo o conteúdo e apague
5. Cole o conteúdo do arquivo `README.md` deste template
6. Clique em **Commit changes**
7. Adicione uma mensagem como: `docs: add profile README`
8. Clique em **Commit changes** novamente

### Opção B — Via terminal (Git)

```bash
# Clone o repositório
git clone https://github.com/SEU_USERNAME/SEU_USERNAME.git

# Entre na pasta
cd SEU_USERNAME

# Copie o README.md do template para esta pasta
# Edite o arquivo com seu editor favorito

# Suba as alterações
git add README.md
git commit -m "docs: add profile README"
git push origin main
```

---

## 4. Substituindo os campos

Todos os campos que precisam ser alterados estão marcados com `SEU_`. Use **Ctrl+H** (ou Cmd+H no Mac) para substituir de uma vez.

| Campo | O que colocar | Onde encontrar |
|-------|--------------|----------------|
| `SEU%20NOME` | Seu nome com espaços trocados por `%20` | Ex: `João%20Silva` |
| `SEU_USERNAME` | Seu usuário do GitHub | Aparece na URL: `github.com/SEU_USERNAME` |
| `SEU_EMAIL` | Seu e-mail profissional | — |
| `SEU_LINKEDIN` | Seu ID do LinkedIn | URL do seu perfil: `linkedin.com/in/SEU_ID` |
| `SEU_ID` | Seu ID do Stack Overflow | URL do seu perfil: `stackoverflow.com/users/SEU_ID` |

> ⚠️ O campo `SEU_USERNAME` aparece **várias vezes** no arquivo. Use a substituição em massa para não perder nenhum.

---

## 5. Personalizando as badges de skills

As badges são geradas pelo serviço [shields.io](https://shields.io). O padrão é:

```
https://img.shields.io/badge/NOME-COR?style=for-the-badge&logo=LOGO&logoColor=white
```

### Para adicionar uma nova badge:

1. Acesse [simpleicons.org](https://simpleicons.org) e procure o logo da tecnologia
2. Copie o nome exato do logo (ex: `react`, `docker`, `python`)
3. Monte a URL substituindo `NOME`, `COR` e `LOGO`

**Exemplos prontos para copiar:**

```markdown
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
```

### Para remover uma badge:

Apague a linha inteira que começa com `![NomeDaTecnologia]`.

---

## 6. Configurando as estatísticas automáticas

As estatísticas são geradas por serviços gratuitos que leem seus dados públicos do GitHub. Basta substituir `SEU_USERNAME` e elas atualizam automaticamente todo dia.

### Stats gerais
```
https://github-readme-stats.vercel.app/api?username=SEU_USERNAME
```
Mostra: commits, PRs, issues, stars e ranking percentual.

### Linguagens mais usadas
```
https://github-readme-stats.vercel.app/api/top-langs/?username=SEU_USERNAME
```
Mostra: as linguagens dos seus repositórios públicos em formato de gráfico.

### Streak (sequência de contribuições)
```
https://nirzak-streak-stats.vercel.app/?user=SEU_USERNAME
```
Mostra: contribuições totais, streak atual e maior streak.

### Contador de visitantes
```
https://api.visitorbadge.io/api/visitors?path=https://github.com/SEU_USERNAME/SEU_USERNAME
```
Conta quantas pessoas visitaram seu perfil.

> 💡 **Personalizando o tema:** todos os serviços aceitam o parâmetro `&theme=`. Temas disponíveis: `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`, `onedark`, `cobalt`, `synthwave`, `highcontrast`, `dracula`.

---

## 7. Configurando a Snake de contribuições

A snake é uma animação que transforma seu gráfico de contribuições em uma cobrinha comendo os quadradinhos. É o elemento mais chamativo do perfil — mas requer uma configuração extra.

### Passo 1 — Criar o arquivo de workflow

Dentro do seu repositório especial (`SEU_USERNAME/SEU_USERNAME`), crie a seguinte estrutura de pastas e arquivo:

```
.github/
  workflows/
    snake.yml
```

### Passo 2 — Conteúdo do arquivo `snake.yml`

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"   # Roda todo dia à meia-noite
  workflow_dispatch:        # Permite rodar manualmente
  push:
    branches:
      - main

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10

    steps:
      - name: Generate snake animation
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Push animation to output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Passo 3 — Ativar permissões do workflow

1. No seu repositório, vá em **Settings → Actions → General**
2. Em **Workflow permissions**, selecione **Read and write permissions**
3. Clique em **Save**

### Passo 4 — Rodar o workflow pela primeira vez

1. Vá em **Actions** no seu repositório
2. Clique em **Generate Snake** na lista da esquerda
3. Clique em **Run workflow → Run workflow**
4. Aguarde alguns segundos — quando o círculo ficar verde ✅, a snake foi gerada

Após isso, ela atualiza automaticamente todo dia à meia-noite.

> ⚠️ Se o círculo ficar vermelho ❌, provavelmente faltou ativar as permissões do Passo 3.

---

## 8. Dicas finais para se destacar

**✅ Mantenha atualizado**
Recrutadores percebem quando o README está com tecnologias que você não usa mais. Revise a cada novo semestre ou projeto.

**✅ Adicione projetos em destaque**
Você pode fixar até 6 repositórios no seu perfil. Escolha os que melhor representam sua evolução técnica.

**✅ Use o tema consistente**
Defina uma cor e tema e use em todos os componentes. No template, o padrão é `theme=dark` com `bg_color=151515`.

**✅ Menos é mais**
Um README limpo e organizado impressiona mais do que um cheio de GIFs e animações desnecessárias.

**✅ Commit com frequência**
O gráfico de contribuições (e a snake) ficam mais impressionantes com commits diários — mesmo que pequenos.

**✅ README ≠ currículo completo**
O objetivo é despertar curiosidade, não listar tudo. Deixe os detalhes para o LinkedIn e as entrevistas.

---

> Feito com 💛 por **Adryann Felix**  
> [github.com/Adryannofc](https://github.com/Adryannofc) · [linkedin.com/in/adryann-felix-7a3b4925b](https://linkedin.com/in/adryann-felix-7a3b4925b)
