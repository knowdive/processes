# Processes
In this repository you can find 2 RapidMiner's Processes:
 - KnowledgeScraper: this Process will scrape LOV to get information about the versions and about the latest version of the vocabularies and their relative MetaData
 - KnowledgeParser: this Process will parse the vocabularies given as input with their relative MetaData:
    - it saves a Excel File containing all the triples for each vocabulary (eventually filtering on the predicates) (also with inheritance)
    - it stores a .rdf, .n3, .nt, .json-ld, .ttl serialized version of each vocabulary
    - it saves a Excel Files containing all the triples of every vocabulary (eventually filtering on the predicates) (also with inheritance)
    - it saves a CSV File containing all the triples of every vocabulary (eventually filtering on the predicates) (also with inheritance)
    - it serializes vocabularies in the given formats
 - KnowledgeAnalyser: this Process will use the Filtered vocabularies and the list of Predicates(optional) given as input to analyse it and generate more knowledge
 - KnowledgeConverter: this Process will use the CrossData.xlsx file, obtained from KnowledgeAnalyser, to create a new vocabulary, serialized in different formats(.rdf, .n3, .nt, .json-ld, .ttl)
 - KnowledgeEmbedder: this Process will use a csv parsed file to obtain the Knowledge Embedding of the relative parsed Knowledge Graph using the python library pyKEEN
 - OWL2DL: this Process will use the OWL file and returns the .csv and .xlsx containing its relative DL Axioms (only works with outdated RapidMiner+Ontology extension)
 - AlloyConverter: this Process will get the OWL file, related DL Axioms, and Alloy utils files as input and produce as output the desired Alloy specifications
 - AlloyResults2OWL: this Process will get a text file with the result of the Alloy Analyser and add its istances to the OWL given as input
 - OWL2Alloy: this Process will get the OWL file, compute its related DL Axioms, and get the Alloy utils file as input and produce as output the desired Alloy specification

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
    - pykeen
    - numpy
    - ontospy
  - add rmx_ontology = 5.1 and rmx_text = 9.3 as RapidMiner Extensions (for OWL2Alloy)