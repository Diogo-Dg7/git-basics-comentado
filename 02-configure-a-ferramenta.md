# 02. Configure a ferramenta

> Configure informações de usuário para todos os repositórios locais.

> Seção do [GitHub Git Cheat Sheet (pt-BR)](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/).


[⬅ Instale o Git](01-instale-o-git.md) · [Índice](../README.md) · [Crie repositórios ➡](03-crie-repositorios.md)

---

## Comandos desta seção (2)

### 1. `git config --global user.name "[nome]"`

```bash
git config --global user.name "[nome]"
```

**O que faz:**

Configura o nome que você quer ligado às suas transações de commit.
Ele define a identidade visual do autor que aparecerá no histórico do repositório.
Eu usaria logo após instalar o Git em um novo computador para registrar meu nome globalmente.

**Quando usar / observação:**

A opção `--global` aplica a configuração para todos os repositórios do seu usuário no sistema.

---

### 2. `git config --global user.email "[endereco-de-email]"`

```bash
git config --global user.email "[endereco-de-email]"
```

**O que faz:**

Configura o email que você quer ligado às suas transações de commit.
Ele vincula seus commits à sua conta do GitHub ou serviço de hospedagem correspondente.
Eu usaria na configuração inicial do Git para garantir que minhas contribuições sejam associadas ao meu perfil.

**Quando usar / observação:**

Use o mesmo endereço de e-mail cadastrado na sua conta do GitHub.

---

## Checklist deste arquivo

- [X] 1. `git config --global user.name "[nome]"`
- [X] 2. `git config --global user.email "[endereco-de-email]"`

---

[⬅ Instale o Git](01-instale-o-git.md) · [Índice](../README.md) · [Crie repositórios ➡](03-crie-repositorios.md)
