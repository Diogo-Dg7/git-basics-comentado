# 04. Faça mudanças

> Revise edições e crie uma transação de commit.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Crie repositórios](03-crie-repositorios.md) · [Índice](../README.md) · [Mudanças em grupo ➡](05-mudancas-em-grupo.md)

---

## Comandos desta seção (6)

### 1. `git status`

```bash
git status
```

**O que faz:**

Lista todos os arquivos novos ou modificados para serem commitados.
Ele exibe o estado atual da área de trabalho e da staging area (área de preparação).
Eu usaria frequentemente antes de adicionar arquivos ou criar commits para verificar quais arquivos foram alterados.

**Quando usar / observação:**

Comando essencial para ter clareza sobre o estado dos arquivos antes de qualquer alteração no histórico.

---

### 2. `git diff`

```bash
git diff
```

**O que faz:**

Mostra diferenças no arquivo que ainda não foram preparadas.
Ele compara as modificações do diretório de trabalho atual com a staging area.
Eu usaria para revisar exatamente quais linhas de código mudei antes de dar um `git add`.

**Quando usar / observação:**

Útil para evitar incluir alterações indesejadas no staging.

---

### 3. `git add [arquivo]`

```bash
git add [arquivo]
```

**O que faz:**

Faz o snapshot de um arquivo na preparação para versionamento.
Ele move as alterações selecionadas do diretório de trabalho para a staging area.
Eu usaria quando finalizasse a alteração em um arquivo e quisesse prepará-lo para o próximo commit.

**Quando usar / observação:**

Você pode usar `git add .` para preparar todos os arquivos alterados de uma só vez.

---

### 4. `git diff --staged`

```bash
git diff --staged
```

**O que faz:**

Mostra a diferença entre arquivos preparados e suas últimas versões.
Ele compara o que está na staging area com o último commit gravado no repositório.
Eu usaria logo antes de fazer um commit para ter certeza do que será gravado no histórico.

**Quando usar / observação:**

Excelente para fazer a revisão final antes de registrar a mensagem de commit.

---

### 5. `git reset [arquivo]`

```bash
git reset [arquivo]
```

**O que faz:**

Retira o arquivo da área de preparação, mas preserva seu conteúdo.
Ele cancela o `git add` de um arquivo sem perder o código escrito.
Eu usaria se adicionasse um arquivo por engano na staging area e quisesse removê-lo antes de commitar.

**Quando usar / observação:**

Não altera as modificações feitas no arquivo físico, apenas remove o status de preparado (staged).

---

### 6. `git commit -m "[mensagem descritiva]"`

```bash
git commit -m "[mensagem descritiva]"
```

**O que faz:**

Grava o snapshot permanentemente do arquivo no histórico de versão.
Ele salva as alterações preparadas junto com uma mensagem explicativa sobre o que foi feito.
Eu usaria após preparar as alterações necessárias para criar um ponto de restauração no histórico.

**Quando usar / observação:**

Escreva mensagens claras e descritivas para facilitar o entendimento futuro do projeto.

---

## Checklist deste arquivo

- [X] 1. `git status`
- [X] 2. `git diff`
- [X] 3. `git add [arquivo]`
- [X] 4. `git diff --staged`
- [X] 5. `git reset [arquivo]`
- [X] 6. `git commit -m "[mensagem descritiva]"`

---

[⬅ Crie repositórios](03-crie-repositorios.md) · [Índice](../README.md) · [Mudanças em grupo ➡](05-mudancas-em-grupo.md)
