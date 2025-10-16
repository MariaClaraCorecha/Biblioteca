# 📚 Biblioteca em Java

Sistema de gerenciamento de biblioteca desenvolvido em Java, com integração com banco de dados MySQL.  
Permite cadastrar, listar, atualizar e remover livros de forma prática, usando um menu interativo no console.

---

##  Funcionalidades

- Cadastrar livros (título e autor)  
- Listar todos os livros cadastrados  
- Atualizar informações de livros pelo ID  
- Remover livros pelo ID  
- Salvar os dados no banco MySQL, garantindo persistência  

---

##  Tecnologias utilizadas

- **Java** (POO, Scanner, JDBC)  
- **MySQL** (banco de dados relacional)  
- **JDBC** (Java Database Connectivity)  
- IDE: **IntelliJ IDEA** ou **VS Code**  

---

##  Pré-requisitos

Antes de rodar o projeto, você precisa:

1. Ter o **Java JDK** instalado (versão 11 ou superior)  
2. Ter o **MySQL** instalado e em execução  
3. Criar o banco de dados e a tabela:

```sql
CREATE DATABASE biblioteca_db;

USE biblioteca_db;

CREATE TABLE livros (
    id INT AUTO_INCREMENT PRIMARY KEY,
    titulo VARCHAR(100),
    autor VARCHAR(100),
    disponivel BOOLEAN DEFAULT TRUE
);

