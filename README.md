# Processes
In this repository you can find 2 RapidMiner's Processes:
 - KnowledgeScraper_Full: this Process will scrape LOV to get information about the versions and about the latest version of the vocabularies and their relative MetaData
 - KnowledgeParser: this Process will parse the vocabularies given as input with their relative MetaData:
    - it saves a Excel File containing all the triples for each vocabulary
    - it stores a .nt serialized version of each vocabulary
    - it saves a Excel Files containing all the triples of every vocabulary
    - it saves a CSV File containing all the triples of every vocabulary

## HowTo
In order to use those RapidMiner's Processes, you need to:
 - install Python
 - install these libraries:
    - bs4
    - request
    - pandas
    - time
    - re
    - json
    - os
    - rdflib