# Transações e Teste ACID

Transações são utilizadas quando temos a necessidade de assegurar a confiabilidade das operações feitas em um banco de dados.

Pois nos dá garantia de que caso alguma operação falhe, nenhuma alteração é concretizada nas tabelas do banco de dados.

## Principios ACID

Transações seguem o conjunto de princípios ACID.

### Atômicas

As transações devem ser indivisíveis, as partes não podem ser separadas.

### Consistentes

Devem seguir as regras de integridade do BD. Exemplos tipos das colunas.

### Isoladas

Enquanto as atividades de uma transação estão sendo executadas, ninguém pode fazer alterações nos dados envolvidos.

### Duráveis

Assegura que as informações foram realmente alteradas quando é recebida uma confirmação da transação.

## Quando é necessária?

As transações são necessárias quando temos a necessidade de fazer:

-   Multiplas tarefas
-   Ações conjuntas
-   E ter acesso exclusivo as dados.
