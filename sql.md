# SQL

A linguagem de consulta mais comum é a SQL - Linguagem de consulta estruturada.

## RDBMs

Gerenciadores de Banco de Dados Relacionais.

## Nomeclaturas

-   DML - Data Manipulation Language - Interagir com os dados.
-   DDL - Data Definition Language - Gerenciar os bancos de dados
-   DCL - Data Control Language - Gerenciar usuários, criar regras, controlar acesso.

## Instruções

Podem conter:

-   Cláusulas
    -   Expressões
    -   Predicados

### Queries

São solicitações de operações e consultas no banco de dados.

### Exemplos

"Me mostre o nome e email de todas as pessoas que estão na tabela Clientes, e nasceram em 1970."

    SELECT nome, email FROM Clientes
    WHERE YEAR(aniversario) = 1970;

## CRUD - Operações mais comuns

-   C - Create - Criar
-   R - Read - Ler
-   U - Update - Atualizar
-   D - Delete - Remover
