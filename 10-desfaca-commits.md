# 10. Desfaça commits

> Apague enganos e crie um histórico substituto.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Revise o histórico](09-revise-o-historico.md) · [Índice](../README.md) · [Sincronize mudanças ➡](11-sincronize-mudancas.md)

---

## Comandos desta seção (2)

### 1. `git reset [commit]`

```bash
git reset [commit]
```

**O que faz:**

Desfaz todos os commits depois de [commit], preservando mudanças locais.
Ele move a referência da branch de volta para o commit especificado, mantendo todo o código alterado na sua pasta.
Eu usaria para reorganizar ou reescrever commits locais récem-feitos sem perder o trabalho realizado.

**Quando usar / observação:**

Preserva o código alterado no diretório de trabalho como mudanças não preparadas.

---

### 2. `git reset --hard [commit]`

```bash
git reset --hard [commit]
```

**O que faz:**

Descarta todo histórico e mudanças para o commit especificado.
Ele força o repositório a voltar exatamente para o estado do commit indicado, deletando todas as alterações posteriores.
Eu usaria quando quisesse descartar completamente todas as alterações e commits recentes e recomeçar a partir de um ponto antigo.

**Quando usar / observação:**

Atenção: este comando apaga permanentemente o trabalho não salvo posterior ao commit selecionado.

---

## Checklist deste arquivo

- [X] 1. `git reset [commit]`
- [X] 2. `git reset --hard [commit]`

---

[⬅ Revise o histórico](09-revise-o-historico.md) · [Índice](../README.md) · [Sincronize mudanças ➡](11-sincronize-mudancas.md)
