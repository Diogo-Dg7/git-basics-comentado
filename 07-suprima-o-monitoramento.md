# 07. Suprima o monitoramento

> Ignore arquivos e diretórios temporários.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Refatore nomes de arquivos](06-refatore-nomes-de-arquivos.md) · [Índice](../README.md) · [Salve fragmentos ➡](08-salve-fragmentos.md)

---

## Itens desta seção (2)

### 1. Arquivo `.gitignore`

```gitignore
*.log
build/
temp-*
```

**O que este arquivo faz:**

Um arquivo de texto chamado `.gitignore` suprime o versionamento acidental de arquivos e diretórios correspondentes aos padrões especificados.
Ele evita que arquivos temporários, logs de erros e pastas de dependências sejam rastreados pelo Git.
Eu usaria na raiz do repositório para ignorar pastas como `node_modules/`, arquivos `.log` e arquivos de ambiente `.env`.

**Quando usar / observação:**

Deve ser criado e configurado logo no início do desenvolvimento do projeto.

---

### 2. `git ls-files --others --ignored --exclude-standard`

```bash
git ls-files --others --ignored --exclude-standard
```

**O que faz:**

Lista todos os arquivos ignorados neste projeto.
Ele exibe quais arquivos do sistema estão sendo filtrados pelas regras contidas no arquivo `.gitignore`.
Eu usaria para depurar se um arquivo específico está sendo ignorado corretamente pelas regras configuradas.

**Quando usar / observação:**

Útil para verificar se suas regras do `.gitignore` não estão ignorando arquivos importantes por engano.

---

## Checklist deste arquivo

- [X] 1. Arquivo `.gitignore`
- [X] 2. `git ls-files --others --ignored --exclude-standard`

---

[⬅ Refatore nomes de arquivos](06-refatore-nomes-de-arquivos.md) · [Índice](../README.md) · [Salve fragmentos ➡](08-salve-fragmentos.md)
