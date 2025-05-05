# Creating Collections as Data Using Federated Queries

![From LOD to CaD - banner](gh-banner.jpg)

This repository provides a series of **Jupyter notebooks** designed for performing **federated queries** across **Wikidata** and other **linked open data (LOD)** endpoints, with a focus on querying bibliographic and author-related data. 

These notebooks support our paper *From Linked Open Data to Collections as Data: 
A Reproducible Framework Using Federated Queries* and aim to present reproducible examples of query design strategies other than structured real-world use in library and information studies, digital humanities and other domains.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/semanticnoodles/federated-cad/HEAD)

## How to Cite This Work
We recommend you to cite the paper the notebooks are supporting, as well as the repository as a whole. The citation for the paper is:

> Meltem Dişli, Giulia Osti, Richard L. Zijdeman, & Gustavo Candela. (2025). From Linked Open Data to Collections as Data: A Reproducible Framework Using Federated Queries. *Journal*, Volume(Issue), Page range. DOI

While the citation for the repository is available in the [CITATION.cff](CITATION.cff) file. You can also use the following BibTeX entry:

```bibtex
@misc{federated-cad,
 @misc{Meltem_Disli_and_Giulia_Osti_and_Richard_L_Zijdeman_and_Gustavo_Candela_Federated_LOD_Queries_2025,
author = {{Meltem Dişli} and {Giulia Osti} and {Richard L. Zijdeman} and {Gustavo Candela}},
doi = {10.5281/zenodo.XXXXXXX},
month = apr,
title = {{Federated LOD Queries as CaD - Notebooks}},
url = {https://github.com/hibernator11/federated-lod-queries},
year = {2025}
}  
```

## Materials in this Repository

This project contains several sample Jupyter Notebooks pertaining to:

1.  **Query Building**, (4 examples) a query building workflow. [Wikidata_map_viz](notebooks/01-query-building/wikidata-map-viz.md) offers an example of exploratory query that can be run directly on the Wikidata SPARQL endpint, visualising the place of birth of the authors mapped as part of the Spanish Golden Age (`wd:Q530936`). 
2.  **Single Autors Multiple Works** (2 examples) <!-- add explanation of the example -->
3.  **Multiple Authors Multiple Works** (1 example) <!-- add explanation of the example --> 

### LOD Endpoints on Use

Leveraging Wikidata, the SPARQL queries we present are designed to retrieve data from the following endpoints:

\- `BNE`: **Biblioteca Nacional de España**, the Spanish National Library (http://datos.bne.es/sparql). <!-- add link to BNE SPARQL endpoint -->

\- `BNF`: **Bibliothèque nationale de France**, the National Library of France (https://data.bnf.fr/sparql). <!-- add link to BNF SPARQL endpoint -->

\- `BVMC`: **Biblioteca Virtual Miguel de Cervantes**, the Miguel de Cervantes Virtual Library (https://data.cervantesvirtual.com/sparql). <!-- add link to BVMC SPARQL endpoint -->

## Running the Notebooks with Binder

This project includes example Jupyter notebooks that you can run directly in your browser using [Binder](https://mybinder.org/). Click the **Launch Binder** button below to start a live session:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/semanticnoodles/federated-cad/HEAD)

Once Binder finishes loading you will see a file browser on the left-hand side that will allow you to navigate all the notebooks contained in this repository.

### Tips for Using the Notebooks

-  To run all cells at once: click **“Cell” > “Run All”** from the top menu.
-  To step through cell-by-cell: use the ▶️ **Run** button at the top or next to each cell.
-  Feel free to **edit** code or markdown cells and re-run them — your changes are temporary and will not be saved once the session ends or times out (will not affect the repository structure).

## License

[![Licence Creative Commons](https://camo.githubusercontent.com/87c07f8d6b43e5c3a22e2cc80e0e245c5c47a4f370da2c3465a00a4d55a0239a/68747470733a2f2f692e6372656174697665636f6d6d6f6e732e6f72672f6c2f62792f342e302f38307831352e706e67)](http://creativecommons.org/licenses/by/4.0/)
Content is licensed under a [Creative Commons Attribution 4.0 International license](http://creativecommons.org/licenses/by/4.0/).

## Essential References

If we wish to add some essential refs here.<!-- add references to the paper, the notebooks, and any other relevant resources -->
