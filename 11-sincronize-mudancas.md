# 11. Sincronize mudanças

> Registre um repositório remoto e troque o histórico de versão.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Desfaça commits](10-desfaca-commits.md) · [Índice](../README.md)

---

## Comandos desta seção (4)

### 1. `git fetch [nome-remoto]`

```bash
git fetch [nome-remoto]
```

**O que faz:**

Baixe todo o histórico de um repositório remoto.
Ele atualiza as referências do repositório remoto localmente sem alterar ou mesclar nada no seu código de trabalho.
Eu usaria para verificar o que mudou no servidor remoto sem o risco de afetar meu código atual.

**Quando usar / observação:**

Seguro para inspeção prévia antes de incorporar as mudanças com merge.

---

### 2. `git merge [nome-remoto]/[branch]`

```bash
git merge [nome-remoto]/[branch]
```

**O que faz:**

Combina o branch remoto ao branch local atual.
Ele aplica as alterações trazidas pelo `git fetch` diretamente na sua linha de desenvolvimento atual.
Eu usaria em conjunto com o `git fetch` para atualizar minha branch local com as novidades da equipe.

**Quando usar / observação:**

Representa a segunda metade do processo de sincronização de dados remotos.

---

### 3. `git push [alias] [branch]`

```bash
git push [alias] [branch]
```

**O que faz:**

Envia todos os commits do branch local para o GitHub.
Ele publica seus commits locais no servidor remoto para disponibilizar seu trabalho para a equipe.
Eu usaria sempre que finalizasse uma unidade de trabalho e quisesse atualizar o repositório remoto no GitHub.

**Quando usar / observação:**

Exemplo comum: `git push origin main`.

---

### 4. `git pull`

```bash
git pull
```

**O que faz:**

Baixa o histórico e incorpora as mudanças.
Ele realiza os comandos `git fetch` e `git merge` em uma única operação automática.
Eu usaria ao início do dia de trabalho para garantir que meu código local está totalmente atualizado com o GitHub.

**Quando usar / observação:**

É o modo mais rápido e prático de sincronizar a branch local com a remota.

---

## Checklist deste arquivo

- [ ] 1. `git fetch [nome-remoto]`
- [ ] 2. `git merge [nome-remoto]/[branch]`
- [ ] 3. `git push [alias] [branch]`
- [ ] 4. `git pull`

---

[⬅ Desfaça commits](10-desfaca-commits.md) · [Índice](../README.md)
