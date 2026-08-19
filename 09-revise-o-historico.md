# 09. Revise o histórico

> Navegue e inspecione a evolução dos arquivos do projeto.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Salve fragmentos](08-salve-fragmentos.md) · [Índice](../README.md) · [Desfaça commits ➡](10-desfaca-commits.md)

---

## Comandos desta seção (4)

### 1. `git log`

```bash
git log
```

**O que faz:**

Lista o histórico de versões para o branch atual.
Ele mostra a lista cronológica de commits realizados com autor, data e mensagem.
Eu usaria para navegar e inspecionar a evolução do projeto ao longo do tempo.

**Quando usar / observação:**

Adicione a flag `--oneline` para ver o histórico de forma resumida e compacta.

---

### 2. `git log --follow [arquivo]`

```bash
git log --follow [arquivo]
```

**O que faz:**

Lista o histórico de versões para um arquivo, incluindo mudanças de nome.
Ele mostra toda a evolução de um arquivo específico desde sua criação, mesmo que tenha sido renomeado.
Eu usaria para investigar quem e quando realizou alterações em um arquivo específico no passado.

**Quando usar / observação:**

Essencial para entender o contexto histórico de alterações em arquivos específicos.

---

### 3. `git diff [primeiro-branch]...[segundo-branch]`

```bash
git diff [primeiro-branch]...[segundo-branch]
```

**O que faz:**

Mostra a diferença de conteúdo entre dois branches.
Ele compara as alterações e exibe o que existe de diferente entre a ponta de duas linhas de desenvolvimento.
Eu usaria antes de realizar um merge para entender exatamente quais modificações serão incorporadas.

**Quando usar / observação:**

Excelente para fazer code review entre duas ramificações.

---

### 4. `git show [commit]`

```bash
git show [commit]
```

**O que faz:**

Retorna mudanças de metadata e conteúdo para o commit especificado.
Ele exibe os detalhes completos de um único commit, incluindo o autor, a data e o diff detalhado das alterações.
Eu usaria para inspecionar exatamente o que foi modificado em uma revisão específica usando seu hash de commit.

**Quando usar / observação:**

Permite auditar pontualmente o conteúdo de qualquer commit no histórico.

---

## Checklist deste arquivo

- [X] 1. `git log`
- [X] 2. `git log --follow [arquivo]`
- [X] 3. `git diff [primeiro-branch]...[segundo-branch]`
- [X] 4. `git show [commit]`

---

[⬅ Salve fragmentos](08-salve-fragmentos.md) · [Índice](../README.md) · [Desfaça commits ➡](10-desfaca-commits.md)
