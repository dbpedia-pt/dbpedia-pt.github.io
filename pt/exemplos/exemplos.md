---
layout: page
title: Exemplos
permalink: /exemplos/
---

Nesta página nós vamos demonstrar várias formas de se interagir com a DBpedia, assim como descrever algumas aplicações que se beneficiaram dos dados da DBpedia Português.

## Comece a explorar

Veja o que já conseguimos extrair sobre o [Brasil](http://pt.dbpedia.org/resource/Brasil){:target="_blank"}, por exemplo.
Para isso, vá ao endereço [http://pt.dbpedia.org/resource/Brasil](http://pt.dbpedia.org/resource/Brasil){:target="_blank"}. 
Aproveite para clicar em [outras entidades relacionadas ao Brasil](http://pt.dbpedia.org/resource/Dilma_Rousseff){:target="_blank"} e explorar a interconectividade dos dados ligados extraídos da Wikipedia.

Você também pode executar consultas como se a enciclopédia fosse um banco de dados.
Para isso usamos SPARQL, uma linguagem de consulta RDF que é parecida com o SQL. 
Por exemplo, para encontrar todos os presidentes que tem como religião o catolicismo, pode-se formular a seguinte consulta em SPARQL:

    PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
    PREFIX dbpedia-owl:<http://dbpedia.org/ontology/>

    SELECT DISTINCT ?presidente WHERE {
      ?presidente a dbpedia-owl:President .
      ?presidente dbpedia-owl:religion <http://pt.dbpedia.org/resource/Catolicismo> .
    }

<form method="GET" action="http://pt.dbpedia.org/sparql">
<input type="hidden" name="query" value=" PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
    PREFIX dbpedia-owl:<http://dbpedia.org/ontology/> SELECT DISTINCT ?presidente WHERE { ?presidente a dbpedia-owl:President .  ?presidente dbpedia-owl:religion <http://pt.dbpedia.org/resource/Catolicismo> .  } " />
<input type="submit" value="Executar" /> 
</form>

Clique no botão acima para executar essa consulta e visualizar os resultados em uma tabela. É possível que os resultados retornados estejam incompletos ou até mesmo incorretos. Isso pode ser devido a erros na Wikipedia (de onde extraímos os dados), ou pode ser que algum erro tenha acontecido no processo automático de extração. Por isso é importante mantermos as atividades de [avaliação da qualidade](/como_participar/qualidade) para que a DBpedia fique cada vez mais completa e correta. 

## Outros exemplos:

### Educação

Este é um pequeno exercício para demonstrar a utilidade do conceito de Dados Ligados (Linked Data) como base para o compartilhamento de dados (governamentais) abertos. 
Nosso caso de uso é o da avaliação do envolvimento de representantes do povo brasileiro na solução de problemas eminentes em sua região de origem. Tomamos como exemplo a educação, e buscamos políticos que vem de estados com alto índice de analfabetismo e que envolvem-se com projetos relacionados à educação. O índice de analfabetismo é extraído da Wikipedia pelo projeto DBpedia Portuguese, enquanto as votações de políticos são obtidas do projeto Ligado Nos Políticos. Você pode ver como esse exemplo foi executado a partir da página do exemplo.
