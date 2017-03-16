---
layout: page
title: Integração de Dados
permalink: /como_participar/integracao
lang: pt
---


A Integração de Dados consiste em combinar dados provenientes de fontes de dados distintas de forma a prover uma visão unificada destes dados. 

Um de nossos objetivos é integrar a DBpedia com o maior número possível de fontes de dados, de forma a servir como um núcleo para a Web de Dados, como se pode notar na figura abaixo (criada por Richard Cyganiak and Anja Jentzsch).

<p><a href="http://lod-cloud.net/"><img width="75%" height="75%" src="http://lod-cloud.net/versions/2014-08-30/lod-cloud_colored_1000px.png" title="http://lod-cloud.net"></a></p>

## Como participar?

Se você se interessa em auxiliar na integração de dados com a DBpedia, o primeiro passo é se inscrever na lista e enviar um e-mail se apresentando. Mais detalhes em [Como Participar?](../como_participar)

Como segundo passo, eu sugiro identificar uma área temática, e de preferência já escolher quais conjuntos de dados externos você vai integrar. Bons lugares para começar:

* http://dados.gov.br
* http://datahub.io/dataset?q=brazil

Como terceiro passo, explore os dados existentes na DBpedia para sua área temática. Pode servir de inspiração. Compare os valores na DBpedia e na Wikipedia. A intenção é extrair todos os dados dos Infoboxes para a DBpedia. Às vezes falha, e vale a pena olhar os [mapeamentos](http://mappings.dbpedia.org){:target="_blank"} que geraram os dados para entender os motivos.

O quarto passo pode ser ver quais sobreposições já existem entre os dados que você escolheu e os dados da DBpedia. Para isso, você pode consultar a DBpedia via SPARQL (http://pt.dbpedia.org/sparql) ou navegar os dados ligados (http://pt.dbpedia.org/resource/Brasil), assim como a Wikipedia (http://pt.wikipedia.org/wiki/Brasil). Procure identificadores (URIs) e atributos na fonte de dados que você escolheu que possam estar presentes na DBpedia. Eles servirão como "cola" para a integração.

Finalmente, faça alguns testes. Considere utilizar o Silk, R2R, [Linked Data Integration Framework (LDIF)](http://ldif.wbsg.de/){:target="_blank"} ou outra ferramenta existente. Os resultados de uma tarefa de integração de dados no contexto de RDF são uma série de links <code>owl:sameAs</code>, <code>skos:exactMatch</code>, <code>owl:equivalentClass</code>, <code>rdfs:subclassOf</code> e outras propriedades relacionadas.

Para mais informações, veja: <a href="http://wiki.dbpedia.org/services-resources/interlinking">Interlinking</a> (em inglês)

