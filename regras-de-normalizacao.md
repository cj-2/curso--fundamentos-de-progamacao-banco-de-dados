# Regras de Normalização

São referentes a redundância e integridade dos dados.

- Primeira Forma Normal
- Segunda Forma Normal
- Terceira Forma Normal
- ...

Essas regras devem sempre serem usadas pois são consideradas um padrão de otimização
para um banco de dados comercial.

- Devem ser usadas para qualquer banco de dados criados.
- São critérios formais.
- Devem ser aplicadas em sequencia.

## Primeira Forma Normal

Uma tabela está na 1FM se, e somente se, todos os valores das colunas da tabela forem atômicos.

- Cada campo ou célula deve ter apenas um valor.
- Colunas não devem ser repetidas.
- Colunas não devem conter informações semelhantes.
- Linhas da tabela devem ser únicas
- A ordenação das linhas e colunas não são importantes.

### Erros comuns:

- Lista de valores separados por vírgulas: a, b, c, ...
- Colunas com números no nome: coluna1, coluna2, ...

## Segunda Forma Normal

Atributos da tabela dependem da chave completa e não de parte da chave.

- Todos os atributos não chave, dependem da chave-primária inteira.
- Problema existe apenas com chaves compostas.
- Um valor não pode depender de parte da chave.

## Terceira Forma Normal

Não se pode determinar o valor de um atributo baseado no valor de uma coluna não-chave.

## Desnormalização

Processo de duplicar informações intencionamento para atender requisitos de desempenho.

### Quando pode ser viável?

- Banco de dados muito grandes.
- Servidores lentos.
- Volume grande de requisições simultâneas.
- Verificar se há ganhos de eficiência.
- Ganho de velocidade vs. redução de consistência.
- Decisões que devem ser baseadas nos requisitos de negócio.