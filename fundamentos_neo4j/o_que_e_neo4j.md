# O que é o Neo4j?

Bancos de dados gráficos são particularmente úteis quando as conexões entre os dados são tão importantes quanto os dados em si.

Nós, relacionamentos, rótulos e propriedades
Os dados no Neo4j são armazenados e organizados usando:

- Nós

- Relacionamentos

- Etiquetas

- Propriedades

## Nós
Os nós são os círculos em um gráfico. Os nós geralmente representam objetos ou entidades .

## Etiquetas (Labels)
Os nós são agrupados por ou categorizados usando rótulos . Os rótulos descrevem o que os nós são, por exemplo, Person, Company, Location.

Nós do mesmo tipo teriam o mesmo rótulo.

Os rótulos permitem distinguir entre diferentes tipos de nós e filtrar o gráfico.

Os nós podem ter vários rótulos, por exemplo, Michael é um Persone também pode ser um Employee.

Use substantivos para rótulos

Os nós geralmente representam coisas e devem receber um rótulo de substantivo singular. Por exemplo, Product, Event, Account.

## Relacionamentos

Um relacionamento no Neo4j conecta dois nós, chamados de nós inicial e final .

Todos os relacionamentos têm:

- um tipo - WORKS_AT, FOUNDED_IN.

- uma direção - Michael WORKS_ATNeo4j, Neo4j não funciona em Michael.

Os nós podem ter vários relacionamentos com outros nós.

Vários relacionamentos podem ser usados para descrever relacionamentos bidirecionais.

**Use verbos para tipos de relacionamento**

> Você pode usar um relacionamento para representar:
> 
> - Uma conexão pessoal - Person KNOWS Person, Person MARRIED_TO Person.
> 
> - Um fato - Person LIVES_IN Location, Person OWNS Car, Person RATED Movie.
> 
> - Uma hierarquia - Parent PARENT_OF Child, Software DEPENDS_ON Library.
> 
> - Qualquer tipo de conexão entre 2 entidades - Entity CONNECTED_TO Entity.

## Propriedades

Você pode armazenar dados em nós e relacionamentos como propriedades.

Propriedades são chamadas de pares chave-valor; por exemplo, firstName , lastName e position 

![props](/imagens/node-properties.svg)

Nós e relacionamentos podem ter qualquer número de propriedades, e aqueles do mesmo tipo não precisam ter as mesmas propriedades (ou seja, o Neo4j não tem esquema).

Propriedades têm um tipo (inteiro, booleano, string, lista, etc.) e podem ser identificadores exclusivos (chaves) para rótulos de nós específicos.

