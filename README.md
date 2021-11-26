# Swiss Parliamentary Services Opendata portal
The Parliamentary Services of the Federal Assembly (Bern, Switzerland) have an opendata portal at the address http://ws-old.parlament.ch. Here we present and update on a regular schedule all the data available in JSON format from the Parliamentary Services Opendata portal.

According to the Parliamentary Services, the opendata portal ws-old.parlament.ch will be fully renewed in 2022. 

## Changes with respect to the original data
- JSON objects are prettified in order to take advantage of git to track changes.
- In order to keep directories reasonably small, affairs file names use the following notation ``/#{product}/#{id[0..3]}/#{id[0..3]}-#{id[4]}/#{id}.#{lang}.json``
- The portal API always returns a document even when it is not available in the requested language (fallback to another version). During the crawling phase, documents that do not match the requested language are discarded and are not included in the repository. 

## Additional files
- For each product a ``/#{product}/updates.json`` file is preriodically generated.
- For those products presenting metadata in the index page not included in the JSON objects itself, additional index files are generated: ``/#{product}/index.#{lang}.json``

## Feedbacks
Feedbacks are welcome [@gamba](https://github.com/gamba). For missing or incorrect data open an issue. 

## References, terms and conditions
- https://www.parlament.ch/en/services/open-data-webservices
- https://www.parlament.ch/centers/documents/de/kurzdokumentation-webservices-d.pdf (in german)
- https://www.parlament.ch/en/services/terms-and-conditions

 This repository is licensed under the [CC BY-NC-SA 4.0 licence](https://creativecommons.org/licenses/by-nc-sa/4.0/) and cannot be used for commercial purposes. 
 
 Droid Factory.
