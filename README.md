# pubmed_list_generator

A webpage which contains javascript which will automatically display a list of publications from the [PubMed](https://pubmed.ncbi.nlm.nih.gov/) database.


## Usage
Search terms are entered on line 26. For example:
```var searchterm = "&term=Neher[Author] AND Marty[Author])";``` will search for publications by authors Neher and Marty. Search terms can be found in the PubMed [tutorial](https://www.ncbi.nlm.nih.gov/books/NBK3827/#pubmedhelp.Search_Field_Descriptions_and).

The output format can be changed on line 18:
```var HTMLpublication = '%authors% (%date%) \'%title%\' <i>%journal%\</i>,<b>%volume%</b> %issue%%pages%PMID:<a href="%data%"target="_blank"> %PMID% </a>'``` will generate a reference:
Author AB, (Year) 'Title' *Journal*, **Volume** (issue) pages, PMID: [12345](number)


See my [website](www.ephys.org/ESP32) for a basic example.

## License
The project is distributed under MIT License
