# federated-cad
Example of federated repositories to extract collections as data


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hibernator11/federated-cad/HEAD)


### Example of visualisation

An example of [map visualisation](https://w.wiki/DVyD) using as a main repository Wikidata, the Spanish Golden Age as a movement and the place of birth of the authors provided by repositories National Library of Spain, the National Library of France and Biblioteca Virtual Miguel de Cervantes. 

```

#defaultView:Map 
SELECT distinct ?author ?authorLabel ?location
WHERE{
{
  SELECT distinct ?author ?authorLabel ?location
  WHERE {
    ?author wdt:P950 ?id .
    ?author wdt:P135 wd:Q530936 .
    ?author rdfs:label ?authorLabel.  FILTER(LANG(?authorLabel) = "en").
    ?author wdt:P19 ?birth .
    ?birth wdt:P625 ?location.
  } LIMIT 20000
}
UNION 
{
 SELECT distinct ?author ?authorLabel ?location
 WHERE {
  ?author wdt:P268 ?id .
  ?author wdt:P135 wd:Q530936 .
  ?author rdfs:label ?authorLabel.  FILTER(LANG(?authorLabel) = "en").
  ?author wdt:P19 ?birth .
  ?birth wdt:P625 ?location.
 } LIMIT 20000
}
  UNION 
{
 SELECT distinct ?author ?authorLabel ?location
 WHERE {
  ?author wdt:P2799 ?id .
  ?author wdt:P135 wd:Q530936 .
  ?author rdfs:label ?authorLabel.  FILTER(LANG(?authorLabel) = "en").
  ?author wdt:P19 ?birth .
  ?birth wdt:P625 ?location.
 } LIMIT 20000
}
}
```
