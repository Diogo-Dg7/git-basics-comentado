# 08. Salve fragmentos

> Arquive e restaure mudanças incompletas.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Suprima o monitoramento](07-suprima-o-monitoramento.md) · [Índice](../README.md) · [Revise o histórico ➡](09-revise-o-historico.md)

---

## Comandos desta seção (4)

### 1. `git stash`

```bash
git stash
```

**O que faz:**

Armazena temporariamente todos os arquivos monitorados modificados.
Ele limpa as alterações não commitadas do diretório de trabalho e as guarda em uma pilha temporária.
Eu usaria para mudar rapidamente de branch para corrigir um bug sem precisar fazer um commit incompleto.

**Quando usar / observação:**

Ótimo para interromper o trabalho atual com segurança sem poluir o histórico de commits.

---

### 2. `git stash pop`

```bash
git stash pop
```

**O que faz:**

Restaura os arquivos recentes em stash.
Ele aplica as últimas alterações salvas na pilha do stash e as remove da lista temporária.
Eu usaria ao retornar para a branch original para continuar o trabalho que havia pausado anteriormente.

**Quando usar / observação:**

Aplica as mudanças mais recentes e apaga o registro do stash automaticamente.

---

### 3. `git stash list`

```bash
git stash list
```

**O que faz:**

Lista todos os conjuntos de alterações em stash.
Ele exibe todos os fragmentos salvos temporariamente na pilha com seus respectivos identificadores.
Eu usaria caso tivesse feito vários stashes e precisasse identificar qual deles deseja restaurar.

**Quando usar / observação:**

Mostra os registros gravados no formato `stash@{0}`, `stash@{1}`, etc.

---

### 4. `git stash drop`

```bash
git stash drop
```

**O que faz:**

Descarta os conjuntos de alterações mais recentes em stash.
Ele deleta permanentemente o último registro salvo na pilha de stash sem aplicá-lo ao diretório de trabalho.
Eu usaria se decidisse descartar as alterações temporárias guardadas no stash que não seriam mais úteis.

**Quando usar / observação:**

Cuidado: uma vez executado, o conjunto de alterações descartado não poderá ser recuperado.

---

## Checklist deste arquivo

- [X] 1. `git stash`
- [X] 2. `git stash pop`
- [X] 3. `git stash list`
- [X] 4. `git stash drop`

---

[⬅ Suprima o monitoramento](07-suprima-o-monitoramento.md) · [Índice](../README.md) · [Revise o histórico ➡](09-revise-o-historico.md)
