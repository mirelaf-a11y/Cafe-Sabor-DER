# Cafe-Sabor-DER# Sistema Café Aroma e Sabor

## Visão Geral

O **Café Aroma e Sabor** é um sistema web desenvolvido com **Spring Boot**, voltado para o controle de estoque de produtos de uma cafeteria. O sistema permite o cadastro de produtos, o registro de movimentações de entrada e saída de estoque, autenticação de usuários e acompanhamento do histórico de movimentações.

---

# Funcionalidades Implementadas

## 1. Autenticação e Controle de Acesso

### Login de usuários
- Tela de login personalizada.
- Autenticação via Spring Security.
- Proteção de todas as rotas da aplicação.
- Redirecionamento automático após autenticação.

### Usuários padrão cadastrados

| Usuário | Senha |
|----------|---------|
| admin | admin123 |
| joao.silva | senha123 |

### Recursos de segurança
- Senhas criptografadas com BCrypt.
- Logout seguro.
- Controle de acesso baseado em autenticação.

---

## 2. Gestão de Produtos

### Cadastro de produtos

Permite registrar:

- Nome
- Descrição
- Estoque mínimo
- Lote
- Data de validade
- Quantidade atual

### Listagem de produtos

Exibe todos os produtos cadastrados no sistema.

### Alteração de produtos

Permite atualizar:

- Nome
- Descrição
- Estoque mínimo
- Lote
- Validade
- Quantidade disponível

### Exclusão de produtos

Permite remover produtos cadastrados.

---

## 3. Controle de Estoque

### Registro de Entrada

Permite registrar entrada de mercadorias.

Exemplos:

- Compra de novos produtos
- Reposição de estoque
- Ajustes positivos

### Registro de Saída

Permite registrar:

- Vendas
- Perdas
- Descartes
- Ajustes negativos

### Validações

O sistema valida:

- Quantidade maior que zero
- Existência do produto
- Disponibilidade em estoque para saídas

---

## 4. Histórico de Movimentações

Cada movimentação registra:

- Produto movimentado
- Usuário responsável
- Tipo da movimentação
- Quantidade
- Data e hora da operação

### Tipos de movimentação

- ENTRADA
- SAIDA

### Benefícios

- Rastreabilidade completa
- Auditoria das operações
- Histórico permanente

---

## 5. Dashboard de Estoque

A tela principal de estoque apresenta:

### Indicadores

- Total de produtos cadastrados
- Total de entradas
- Total de saídas

### Informações operacionais

- Lista de produtos
- Histórico de movimentações
- Dados atualizados em tempo real

---

## 6. Persistência de Dados

### Entidades do Sistema

#### Usuário

Campos principais:

- id
- nome
- login
- senha

#### Produto

Campos principais:

- id
- nome
- descrição
- estoque mínimo
- lote
- data de validade
- quantidade atual

#### Movimentação de Estoque

Campos principais:

- id
- tipo de movimentação
- quantidade
- data da movimentação
- produto
- usuário

---

## 7. Relacionamentos

### Produto → Movimentações

Um produto pode possuir várias movimentações.

Relacionamento:

```text
Produto 1 ------ N Movimentações
```

### Usuário → Movimentações

Um usuário pode realizar várias movimentações.

Relacionamento:

```text
Usuário 1 ------ N Movimentações
```

---

## 8. Repositórios Disponíveis

### ProdutoRepository

Funcionalidades:

- Salvar produto
- Buscar por ID
- Listar todos
- Excluir produto
- Buscar por nome
- Buscar produtos com estoque crítico

### UsuarioRepository

Funcionalidades:

- Salvar usuário
- Buscar por login
- Buscar por ID
- Listar usuários

### MovimentacaoEstoqueRepository

Funcionalidades:

- Salvar movimentação
- Buscar histórico
- Buscar por produto
- Buscar por usuário
- Buscar por tipo

---

## 9. Tecnologias Utilizadas

### Backend

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Spring Security

### Banco de Dados

- JPA/Hibernate

### Frontend

- Thymeleaf
- HTML
- CSS

---

## Fluxo Principal do Sistema

```text
Login
   ↓
Tela Inicial
   ↓
Cadastro de Produtos
   ↓
Entrada/Saída de Estoque
   ↓
Histórico de Movimentações
   ↓
Relatórios Operacionais
```

---

## Casos de Uso

### Operador de Estoque

- Fazer login
- Cadastrar produto
- Alterar produto
- Registrar entrada
- Registrar saída
- Consultar histórico

### Administrador

- Todas as funcionalidades do operador
- Gestão completa do estoque

---

## Resumo Executivo

O sistema implementa um fluxo completo de controle de estoque para uma cafeteria, incluindo:

✅ Autenticação de usuários

✅ Cadastro de produtos

✅ Alteração e exclusão de produtos

✅ Controle de entrada e saída

✅ Histórico de movimentações

✅ Persistência em banco de dados

✅ Relacionamentos entre entidades

✅ Segurança com Spring Security

✅ Dashboard operacional de estoque
