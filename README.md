# CeneoScraperCS12

https://www.ceneo.pl/84514582#tab=reviews

## Algorithm for extracting opinions about single product from Ceneo.pl
1. Send the request for accessing first webpage with opinions about product
2. If response is OK, parse HTML page content into DOM structure
3. Extract opinions and their components from DOM structure 
4. Assign opinions with their components to complex data structures
5. If there are more pages with pinions, repeat steps 1-5
6. Save data dtructures with opinions into database

## Structure of single opinion in Ceneo.pl
|Component|Variable|Selector|
|---------|--------|--------|
|opinion|opinion||
|opinion ID|opinion_id||
|opinion’s author|author||
|author’s recommendation|recommend||
|score expressed in number of stars|stars||
|opinion’s content|content||
|list of product advantages|pros||
|list of product disadvantages|cons||
|how many users think that opinion was helpful|up_votes||
|how many users think that opinion was unhelpful|down_votes||
|publishing date|published||
|purchase date|purchased||