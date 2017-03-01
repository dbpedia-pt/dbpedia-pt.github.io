---
layout: post
title:  "Novo realease da DBpedia (2015-10) está disponível para download"
date:   2016-04-01 09:40:00 -0300
comments: true
categories: releases
resume: "Temos orgulho em apresentar a nova versão da DBpedia: 2015-10. Ela está disponível agora no nosso triple store [...]"
lang: pt
---

Temos orgulho em apresentar a nova versão da DBpedia: 2015-10. Ela está disponível agora no nosso triple store [http://dbpedia.org/sparql](http://dbpedia.org/sparql){:target="_blank"}.

Esta versão da DBpedia é baseada nos dumps atualizados da Wikipedia do mês de outubro 2015. Ela contém uma base significativamente expandida de informações, bem como dados mais ricos e mais limpos na base de ontologia da DBpedia.


#### O que há de novo?

A comunidade adicionou novas classes e propriedades a ontologia da DBpedia utilizando o mapping wiki. A versão DBpedia 2015-10 engloba

* 739 classes (DBpedia 2015-04: 735)
* 1,099 object properties (DBpedia 2015-04: 1,098)
* 1,596 datatype properties (DBpedia 2015-04: 1,583)
* 132 datatype properties especializados (DBpedia 2015-04: 132)
* 407 owl:equivalentClass e 222 owl:equivalentProperty mapeados de vocabulários externos  (DBpedia 2015-04: 408 and 200, respectivamente)

Os editores da comunidade definiram também novos mapeamentos a partir dos templates da Wikipedia e das classes  DBpedia. Para a versão DBpedia 2015-10, utilizou-se um total de 5553 mapeamentos de modelo (DBpedia 2015-04: 4317 mapeamentos). Pela primeira vez o idioma Inglês não figurou com o maior número de mapeamentos. O holandês com 606 mapeamentos, superou a comunidade Inglesa com 600 mapeamentos.

#### E quais são as principais mudanças?

* A DBpedia Inglesa passou a utilizar IRIs a partir das URIs. 
* O dataset instance-types foi divido em dois arquivos:
  * “instance-types” contém somentes os tipos diretos.
  * “Instance-types-transitive” contém os tipos transitivos.
  * O arquivo “mappingbased-properties” foi dividido em três arquivos:
	* “geo-coordinates-mappingbased”
	* “mappingbased-literals” contém os mapeamentos baseados em declarações com valores literais.
	* “mappingbased-objects”
* Adicionou-se um novo extrator para citações.
* Todos os datasets estão disponíveis nos formatos .ttl e.tql 
* A DBpedia agora é também distribuida via [Docker](https://github.com/dbpedia/Dockerized-DBpedia){:target="_blank"}.
* A partir de agora, iremos fornecer um dataset com os metadados que conterá os DataIDs para todos os idiomas extraídos em suas respectivas pastas.

Além disso, modificamos a tabela dos datasets na página de download. A mesma é criada dinamicamente com base na identificação dos dados de todas as línguas. Da mesma forma, as tabelas na página de Estatísticas, que agora são baseados em arquivos  e fornecem informações sobre todos os idiomas mapeados.

Vale ressaltar que nós iremos incluir o dump original Wikipedia (‘pages_articles.xml.bz2') em conjunto com os dados extraídos. O [changelog completo](https://github.com/dbpedia/extraction-framework/compare/DBpedia_2015-04...master){:target="_blank"} pode ser encontrado no git.

#### E sobre os números da DBpedia?
No total, a nova versão da DBpedia consite em 8.8 bilhões de triplas RDF ( a versão 2015-04 continha 6.9 bilhões), dos quais 1.1 bilhão (2015-04: 737 milhões) foram extraídas da edição Inglesa da Wikipedia, 4.4 bilhões (2015-04: 3.8 bilhões) foram extraídos de outros idiomas e 3.2 bilhões (2015-04: 2.4 bilhões) vieram do projeto DBpedia Commons e Wikidata. No geral, observou-se um crescimento de aproxidamente 10% de infoxboxes e declarações baseadas em mapeamentos.  Esta informação completa você pode encontrar na página de [estatísticas (em inglês)](http://wiki.dbpedia.org/services-resources/datasets/dataset-2015-10/dataset-2015-10-statistics){:target="_blank"}.

#### E o que está por vir?

Nós continuamos a trabalhar no mappings wiki e teremos pelo menos mais um sprint de mapemento este ano. Além disso, temos algumas novas idéias para o GSoC 2016. Novos mentores são sempre bem vindos! :-)

#### E quem contribuiu para esta nova versão?

Gostaríamos de agradecer a todos os editores de mapeamento que constribuiram via the Mappings Wiki, todos os estudantes que participaram do  GSoC e os mentores  que trabalharam direta ou indiretamente nesta nova versão da DBpedia release, além do comitê de internacionalização por promover a DBpedia.

Agradecemos especialmente ao Markus Freudenberg e Dimitris Kontokostas (Universidade de Leipzig), Volha Bryl (Universidade de Mannheim / Springer), Heiko Paulheim (Universidade de  Mannheim), Václav Zeman e todo o time do LHD (Universidade de  Prague), Marco Fossati (FBK), Alan Meehan (TCD), Aldo Gangemi (Universidade LIPN, França & ISTC-CNR, Itália), Kingsley Idehen, Patrick van Kleef, e Mitko Iliev [OpenLink Software](http://www.openlinksw.com/){:target="_blank"}, Ruben Verborgh da Universidade de Ghent – iMinds, Ali Ismayilov (Universidade de Bonn), Vladimir Alexiev (Ontotext) e os membros da DBpedia Association, além do grupo AKSW e do departamento de Business Information Systems da Universidade de Leipzig por seu compromisso em investir tempo e esforço para obter este feito.

Todo o trabalho na versão  DBpedia 2015-10 foi financiado pela Comissão Européia através do projeto [ALIGNED – quality-centric, software and data engineering](http://aligned-project.eu/){:target="_blank"}.
 

Informações detalhadas acerca da nova versão estão disponíveis [aqui](). Para mais informações sobre a DBpedia, por favor, visite nosso [website](http://www.dbpedia.org){:target="_blank"} ou nos acompanhe no [Twitter](https://twitter.com/dbpedia){:target="_blank"} ou [Facebook](https://www.facebook.com/dbpedia.org/){:target="_blank"}.



Atenciosamente,

DBpedia Association

