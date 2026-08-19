# 05. Mudanças em grupo

> Nomeie uma série de commits e combine os esforços completos.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Faça mudanças](04-faca-mudancas.md) · [Índice](../README.md) · [Refatore nomes de arquivos ➡](06-refatore-nomes-de-arquivos.md)

---

## Comandos desta seção (5)

### 1. `git branch`

```bash
git branch
```

**O que faz:**

Lista todos os branches locais no repositório atual.
Ele indica em qual branch você está trabalhando no momento com um sinal de asterisco.
Eu usaria para verificar quais branches existem e confirmar em qual delas me encontro antes de trabalhar.

**Quando usar / observação:**

Use `-a` para listar também os branches remotos.

---

### 2. `git branch [nome-do-branch]`

```bash
git branch [nome-do-branch]
```

**O que faz:**

Cria um novo branch.
Ele estabelece uma nova linha de desenvolvimento independente sem alterar a branch atual.
Eu usaria para iniciar o desenvolvimento de uma nova funcionalidade ou correção de bug.

**Quando usar / observação:**

Este comando apenas cria o branch, não muda automaticamente para ele.

---

### 3. `git switch -c [nome-do-branch]`

```bash
git switch -c [nome-do-branch]
```

**O que faz:**

Muda para o branch especificado e atualiza o diretório de trabalho.
Com a flag `-c`, ele cria o branch e já faz a alternância para ele em um único passo.
Eu usaria sempre que precisasse começar a trabalhar imediatamente em um novo branch.

**Quando usar / observação:**

Substitui o comando tradicional `git checkout -b [nome-do-branch]`.

---

### 4. `git merge [nome-do-branch]`

```bash
git merge [nome-do-branch]
```

**O que faz:**

Combina o histórico do branch especificado ao branch atual.
Ele integra o trabalho concluído de outra linha de desenvolvimento na sua branch principal.
Eu usaria para trazer as alterações de uma funcionalidade concluída para a branch `main`.

**Quando usar / observação:**

Certifique-se de estar na branch de destino antes de executar o merge.

---

### 5. `git branch -d [nome-do-branch]`

```bash
git branch -d [nome-do-branch]
```

**O que faz:**

Exclui o branch especificado.
Ele remove uma linha de desenvolvimento que já foi mesclada e não é mais necessária.
Eu usaria após realizar o merge com sucesso de uma funcionalidade concluída.

**Quando usar / observação:**

Ajuda a manter o repositório limpo e organizado.

---

## Checklist deste arquivo

- [X] 1. `git branch`
- [X] 2. `git branch [nome-do-branch]`
- [X] 3. `git switch -c [nome-do-branch]`
- [X] 4. `git merge [nome-do-branch]`
- [X] 5. `git branch -d [nome-do-branch]`

---

[⬅ Faça mudanças](04-faca-mudancas.md) · [Índice](../README.md) · [Refatore nomes de arquivos ➡](06-refatore-nomes-de-arquivos.md)
