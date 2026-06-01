<div align="center">

# 💙💜 Café Aroma e Sabor

### Sistema de Controle de Estoque para Cafeteria

<img src="https://img.shields.io/badge/Spring_Boot-Backend-6A5ACD?style=for-the-badge" />
<img src="https://img.shields.io/badge/Java-17-4169E1?style=for-the-badge" />
<img src="https://img.shields.io/badge/Spring_Security-Segurança-7B68EE?style=for-the-badge" />
<img src="https://img.shields.io/badge/Thymeleaf-Frontend-1E90FF?style=for-the-badge" />

</div>

---

## 🔷 Visão Geral

> Sistema desenvolvido para gerenciamento de estoque de cafeteria, permitindo controle de produtos, movimentações de estoque e autenticação de usuários.

### ✨ Principais Recursos

🔹 Cadastro de Produtos

🔹 Controle de Entradas e Saídas

🔹 Histórico de Movimentações

🔹 Dashboard Operacional

🔹 Autenticação Segura

---

# 💜 Funcionalidades

## 🔐 Autenticação e Segurança

<div style="border-left:4px solid #7B68EE;padding-left:10px;">

✔ Login de usuários

✔ Logout seguro

✔ Proteção de rotas

✔ Senhas criptografadas com BCrypt

✔ Spring Security

</div>

---

## 📦 Gestão de Produtos

| 🔹 Recurso | 🔵 Descrição |
|------------|-------------|
| Cadastro | Inclusão de novos produtos |
| Consulta | Listagem completa |
| Alteração | Atualização de informações |
| Exclusão | Remoção de registros |

---

## 📊 Controle de Estoque

### 📈 Entradas

- Compra de mercadorias
- Reposição de estoque
- Ajustes positivos

### 📉 Saídas

- Vendas
- Perdas
- Descartes
- Ajustes negativos

---

## 📝 Histórico de Movimentações

```text
┌─────────────────────────────┐
│       MOVIMENTAÇÃO          │
├─────────────────────────────┤
│ Produto                     │
│ Usuário                     │
│ Tipo                        │
│ Quantidade                  │
│ Data/Hora                   │
└─────────────────────────────┘
```

---

# 💙 Estrutura do Sistema

## 👤 Usuário

```text
id
nome
login
senha
```

## 📦 Produto

```text
id
nome
descricao
estoqueMinimo
lote
dataValidade
quantidadeAtual
```

## 🔄 Movimentação

```text
id
tipoMovimentacao
quantidade
dataMovimentacao
produto
usuario
```

---

# 💜 Fluxo do Sistema

```text
┌──────────────┐
│ 🔐 Login     │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ 📊 Dashboard │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ 📦 Produtos  │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ 🔄 Estoque   │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ 📝 Histórico │
└──────────────┘
```

---

# 🛠 Tecnologias

| Tecnologia | Finalidade |
|------------|------------|
| ☕ Java | Linguagem |
| 🌱 Spring Boot | Backend |
| 🔐 Spring Security | Segurança |
| 🗃 JPA/Hibernate | Persistência |
| 🎨 Thymeleaf | Frontend |

---

<div align="center">

## 💙💜 Resumo

✅ Autenticação

✅ Cadastro de Produtos

✅ Controle de Estoque

✅ Histórico de Movimentações

✅ Dashboard Operacional

✅ Segurança com Spring Security

---

### 🚀Autora

Projeto desenvolvido para fins acadêmicos no curso de Desenvolvimento de Sistemas SENAI- Mirela Marques de Faria.

### 🚀 Café Aroma e Sabor

</div>
