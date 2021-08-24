# Modelagem ou Schema

-   Definição formal do banco de dados.
-   Inclui todas as tabelas, colunas, chaves primarias e relacionamentos.
-   Seguindo regras, restrições e estruturas para os dados.

## Entity Relationship Diagram

Digrama de relacionamento de entidades.

## Exemplo

### O que nosso banco de dados precisa armazenar?

Um dono de restaurante precisaria armazenar os seguintes dados:

-   Clientes
-   Itens do Cardápio
-   Pratos favoritos
-   Pedidos
-   Reservas

#### Clientes

O que um cliente tem?

-   id
-   nome
-   email
-   telefone
-   aniversario

#### Itens do Cardápio

-   id
-   nome
-   descricao
-   categoria
-   preco

#### Itens Favoritos

-   idCliente
-   idPratofavorito

E por aí vai...

### Sugestões de Nomeclatura

-   Nome da tabela no plural: Clientes, ItensCardapio
-   Não usar nomes genéricos
-   Campos em singular como: nome, email, telefone.
-   CamelCase para colunas.

## Tipos de Dados

-   STRING, VARCHAR - Sequencia de caractéres. Ex: nomes, endereços, descrições...
-   DATE, TIMESTAMP - Data e/ou hora. - Aniversário, criação, alterações...
-   INTEGER, SMALLINT, DECIMAL, NUMERIC - Números com diferentes níves de precisão.

### String

#### CHAR

-   Número fixo de caracteres.
-   Estados (2), Aeroportos(3), ...

#### VARCHAR

-   Número variavel de caracteres, com um limite máximo.
-   Nomes (<255), Descrições (<1500).

### Números

-   INT - Inteiro sem cada decimais. - Número de pessoas, carros, itens em geral...
-   FLOAT - Flutuante com casas decimais. - Dinheiro, medidas, velocidade...
-   DOUBLE - O dobro de precisão do FLOAT. - Raiz quadrada, Pi...
-   ...

#### Números de Telefone

Se armazena números de telefone em uma string como VARCHAR(20).

### NULL

O nulo representa uma ausência de um valor, ou seja, não é vazio e sim nulo.

-   Nulo é uma condição, não um valor.
-   O campo está nulo, ou seja, não tem o valor "nulo".

### Exemplos de uso de tipos

Clientes

-   nome - VARCHAR(200)
-   email - VARCHAR(200)
-   aniversario - DATE
-   horaNacimento - DATETIME
-   dataCriacao - TIMESTAMP
-   dinheiro - DECIMAL(3,2) - (3 inteiros e 2 decimais)

## Chaves

### Chaves Primarias

Chave substituta ou sintética, tem um valor diferente para todos os registros da tabela, ou seja, é unica.

É comum se utilizar números inteiros, mas algumas pessoas por segurança utilizam o UUID - Unique Universal Identifier.

### Chaves Compostas

Chaves compostas são criadas a partir da combinação de 2 ou mais valores de colunas diferentes 
para compor uma "chave primária única".