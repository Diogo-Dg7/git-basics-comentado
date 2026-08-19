# 06. Refatore nomes de arquivos

> Mude e remova os arquivos versionados.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Mudanças em grupo](05-mudancas-em-grupo.md) · [Índice](../README.md) · [Suprima o monitoramento ➡](07-suprima-o-monitoramento.md)

---

## Comandos desta seção (3)

### 1. `git rm [arquivo]`

```bash
git rm [arquivo]
```

**O que faz:**

Remove o arquivo do diretório de trabalho e o prepara a remoção.
Ele deleta o arquivo fisicamente da pasta e já agenda a exclusão para o próximo commit.
Eu usaria quando quisesse apagar definitivamente um arquivo do controle de versão e do projeto.

**Quando usar / observação:**

Equivale a deletar o arquivo manualmente e depois rodar `git add`.

---

### 2. `git rm --cached [arquivo]`

```bash
git rm --cached [arquivo]
```

**O que faz:**

Remove o arquivo do controle de versão mas preserva o arquivo localmente.
Ele faz o Git parar de rastrear o arquivo sem apagá-lo do seu computador.
Eu usaria ao perceber que adicionei sem querer um arquivo de configuração pessoal ou senha ao Git.

**Quando usar / observação:**

Geralmente acompanhado da adição do padrão desse arquivo ao `.gitignore`.

---

### 3. `git mv [arquivo-original] [arquivo-renomeado]`

```bash
git mv [arquivo-original] [arquivo-renomeado]
```

**O que faz:**

Muda o nome do arquivo e o prepara para o commit.
Ele renomeia ou move o arquivo mantendo o histórico de alterações associado a ele.
Eu usaria para renomear arquivos ou movê-los entre diretórios mantendo a rastreabilidade no Git.

**Quando usar / observação:**

Evita que o Git interprete a renomeação como uma exclusão seguida de uma criação de novo arquivo.

---

## Checklist deste arquivo

- [X] 1. `git rm [arquivo]`
- [X] 2. `git rm --cached [arquivo]`
- [X] 3. `git mv [arquivo-original] [arquivo-renomeado]`

---

[⬅ Mudanças em grupo](05-mudancas-em-grupo.md) · [Índice](../README.md) · [Suprima o monitoramento ➡](07-suprima-o-monitoramento.md)
