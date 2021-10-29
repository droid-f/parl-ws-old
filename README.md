# Swiss Parliamentary Services Opendata portal
The Parliamentary Services of the Federal Assembly (Bern, Switzerland) have an opendata portal at the address http://ws-old.parlament.ch. Here we present and update on a regular schedule all the data available on the Parliamentary Services Opendata website.

## Changes with respect to the original data
- JSON objects are prettified in order to take advantage of git to track changes.
- In order to keep directories reasonably small, affairs file names use the following notation ``/#{product}/#{id[0..4]}/#{id}.#{lang}.json``

## Additional files
- For each product a ``/#{product}_updated_at.json`` file is preriodically generated, this helps to keep the dataset up to date without having to scrape the whole website. 
- For those products presenting metadata in the index page not included in the JSON objects itself, additional index files are generated: ``/#{product}/index.#{lang}.json``

## Feedbacks
Feedbacks are welcome. For missing or incorrect data open an issue. 

## References, terms and conditions
- https://www.parlament.ch/en/services/open-data-webservices
- https://www.parlament.ch/centers/documents/de/kurzdokumentation-webservices-d.pdf (in german)
- https://www.parlament.ch/en/services/terms-and-conditions
