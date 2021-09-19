# Lab05 - Marcadores e Taxonomia em Cypher

## Aluno
* `240106`: `Lucas Otávio Nascimento de Araújo`

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução
~~~cypher
MATCH (m:Marcador) --> (c:Categoria {id:"Serviços"})
RETURN c, m
~~~

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução
~~~cypher
MATCH (m:Marcador) --> (c:Categoria {id:"Serviços"})
MATCH (m2:Marcador) --> (c_ch:Categoria) --> (c)
MATCH (m3:Marcador) --> (c_gch:Categoria) --> (c_ch2:Categoria) --> (c)
RETURN c, m, c_ch, m2, c_ch2, c_gch, m3
~~~
