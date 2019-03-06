# Processes
In this repository you can find 3 RapidMiner's Processes:
 - LOV_Scraper_Full: this Process will scrape LOV to get informations about the versions of the vocabularies and their relative MetaData
 - LOV_Scraper_Latest: this Process will scrape LOV to get informations about the latest version of the vocabularies and their relative MetaData
 - vocab_Parser: this Process will parse the vocabularies given as input with their relative MetaData:
    - it saves an Excel File containing all the triples for each vocabulary
    - it stores a .nt serialized version of each vocabulary
    - it save a CSV File containing all the triples of every vocabulary

## HowTo
In order to use those RapidMiner's Processes, you need to:
 - install Python
 - install these libraries:
    - bs4
    - pathlib
    - request
    - pandas
    - time
    - re
    - json
    - os
    - bs4
    - rdflib