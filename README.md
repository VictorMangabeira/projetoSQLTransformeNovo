# 🛒 Projeto de Banco de Dados - Loja

Este projeto foi desenvolvido durante o curso de **Programação de Sistemas** pelo Senac, como parte da formação técnica. O objetivo é estruturar um banco de dados completo para uma loja, incluindo tabelas de funcionários, fornecedores, clientes, usuários, produtos e vendas.

## 📦 Estrutura do Banco de Dados

O banco de dados `dbLoja` contém as seguintes tabelas:

- `tbFuncionarios`: informações dos funcionários da loja
- `tbFornecedores`: dados dos fornecedores
- `tbClientes`: cadastro de clientes
- `tbUsuarios`: usuários do sistema (ligados aos funcionários)
- `tbProdutos`: produtos disponíveis na loja
- `tbVendas`: registro de vendas realizadas

## 🛠️ Tecnologias Utilizadas

- **MySQL**
- **SQL** para criação de tabelas, inserção de dados e relacionamentos

## 📋 Funcionalidades

- Criação e estruturação do banco de dados
- Relacionamento entre tabelas com **chaves estrangeiras**
- Inserção de dados de exemplo
- Visualização da estrutura e dos registros

## 📌 Exemplo de Comando


-- Criar o banco de dados
create database dbLoja;

-- Criar a tabela de funcionários
create table tbFuncionarios(
  codFunc int not null auto_increment,
  nome varchar(100) not null,
  email varchar(100) not null,
  cpf char(14) not null unique,
  ...
  primary key(codFunc)
