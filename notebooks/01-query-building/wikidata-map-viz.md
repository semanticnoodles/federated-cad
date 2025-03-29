# Wikidata Map Visualization Query

This SPARQL query retrieves information about authors associated with the Spanish Golden Age movement (identified by `wd:Q530936`) from Wikidata. It fetches the author's name (`?authorLabel`), their unique identifier, and their birth location (`?location`) with geographic coordinates.

You can run this query in the [Wikidata Query Service](https://query.wikidata.org/) to visualize the data on a map.

## Query
```sparql
PREFIX bne-def: <https://datos.bne.es/def/>
PREFIX dcterms: <http://purl.org/dc/terms/>

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
