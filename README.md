# Processes
In this repository you can find 2 RapidMiner's Processes:
 - KnowledgeScraper: this Process will scrape LOV to get information about the versions and about the latest version of the vocabularies and their relative MetaData
 - KnowledgeParser: this Process will parse the vocabularies given as input with their relative MetaData:
    - it saves a Excel File containing all the triples for each vocabulary (eventually filtering on the predicates) (also with inheritance)
    - it stores a .rdf, .nt, .jsonld, .ttl serialized version of each vocabulary
    - it saves a Excel Files containing all the triples of every vocabulary (eventually filtering on the predicates) (also with inheritance)
    - it saves a CSV File containing all the triples of every vocabulary (eventually filtering on the predicates) (also with inheritance)
 - KnowledgeAnalyser: this Process will use the Filtered vocabularies and the list of Predicates(optional) given as input to analyse it and generate more knowledge

## HowTo
In order to use those RapidMiner's Processes, you need to:
 - install Python >3.7 64-bit
 - install these libraries:
    - bs4
    - request
    - pandas
    - re
    - json
    - rdflib
    - xlrd
    - xlsxwriter
    - networkx