# Consultas

## Ações Comuns

### Criando um Banco de Dados

    CREATE DATABASE Restaurante

### Criando uma Tabela

    CREATE TABLE Clientes (
        id INT(6) NOT NULL AUTO_INCREMENT,
        nome VARCHAR(200) NOT NULL,
        email VARCHAR(255) NOT NULL,
        telefone VARCHAR(255) NOT NULL,
        aniversario DATE NOT NULL,
        PRIMARY KEY (id)
    )

## Comandos Báscios

- CREATE (criar)
- ALTER (alterar)
- DROP (excluir)
- TRUNCATE (esvaziar)
  

- WHERE (onde)
- OR (ou)
- AND (e)
- LIKE (pareça)
- ORDER BY (ordenado por)
  - DESC (descendente)
  - ASC

## Funções Agregadas

- COUNT - Lista a quantidade de itens na consultas.
- SUM - Faz a soma.
- AVG - Retorna a media.
- MIN - Retorna o valor mínimo da consulta.
- MAX - Retorna o valor máximo.

## Juntando Tabelas

    JOIN Clientes ON Clientes.id = Pedidos.clienteId


- ON - Na...
- AS - Como

### Tipos de Junções

- JOIN
- INNER JOIN - Interseção
- LEFT JOIN - Puxa todos dados da tabela da esquerda, juntando com os da direita quando existe paridade.
- RIGHT JOIN - O mesmo do LEFT JOIN mas de forma inversa (tabela da direita que dita as linhas do resultado.)
- UNION - Junção completa de tabelas.

Exemplo de junção completa de tabelas:

    LEFT JOIN UNION RIGHT JOIN

## Inserção de Dados

    INSERT INTO Clientes (nome, email, aniversario, estado)
    VALUES ("Lucas Longo", "lucas@xpto.com", "", "SP")

## Atualizando Dados

    UPDATE Clientes SET email = "jabreu@xyz.com.br" WHERE id = 3

## Remoção de Dados

    DELETE FROM Clientes WHERE id = 3

