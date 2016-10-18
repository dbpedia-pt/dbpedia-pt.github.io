---
layout: page
title: Avaliação de Qualidade
permalink: /como_participar/qualidade
---


Obviamente, uma forma de contribuir com a DBpedia é aumentar a quantidade de dados. O que fazemos é listar os mapeamentos já existentes em [http://mappings.dbpedia.org/server/statistics/pt/](http://mappings.dbpedia.org/server/statistics/pt/){:target="_blank"} e verificar se estão mapeados para as classes e propriedades corretas. Em alguns casos é necessário criar uma nova propriedade para guardar um dado não previsto no modelo atual da DBpedia.
Entretanto, além de buscar sempre aumentar a variedade e quantidade de informações na DBpedia, outra forma muito importante de se melhorar nosso projeto é através da avaliação da qualidade da extração de dados.
Uma forma simples de se avaliar a qualidade é através da inspeção manual. 

Pegue uma página de seu interesse (ex: [http://pt.wikipedia.org/wiki/Pelé](http://pt.wikipedia.org/wiki/Pel%c3%a9){:target="_blank"}), e depois confira se foi tudo extraído corretamente ([http://pt.dbpedia.org/resource/Pelé](https://pt.wikipedia.org/wiki/Pel%C3%A9){:target="_blank"}). Compare com a DBpedia internacional ([http://dbpedia.org/resource/Pelé](http://dbpedia.org/resource/Pel%c3%a9){:target="_blank"}). Repita isso pra uns 10 tipos de entidades diferentes (universidades, carros, pessoas, etc.). 


Se algo não foi extraído, eu olho qual infobox foi usado (no source da Wikipedia), qual mapeamento foi usado (em mappings.dbpedia.org) e tento consertar. O histórico da página da Wikipedia também ajuda a entender muitos problemas, pois as vezes os dados não estavam ainda presentes quando a extração rodou. Acho que cada parceiro deveria ao menos gerar uns mapeamentos e avaliar a qualidade de alguns dados, para que todos conheçam o projeto melhor.
Outra forma simples é através do desenvolvimento de aplicações de demonstração. 


Para demonstrações, eu penso numa pergunta interessante e tento usar a DBpedia para respondê-la. Faço isso através de navegação dos Dados Ligados, e também consultas SPARQL em [http://pt.dbpedia.org/sparql](http://pt.dbpedia.org/sparql){:target="_blank"}) Se os dados estiverem na Wikipedia, mas não na DBpedia, eu tento mapeá-los. Sempre tento também trazer fontes externas e interligar pra tornar as coisas mais interessantes. Veja, por exemplo, o exercício no tema política de educação.


