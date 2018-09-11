# Hermes
Automated process to get information from PubMed into VIVO

Hermes uses the Pubmed api to parse and process publications listed in Pubmed to be uploaded to VIVO.

## Usage
Hermes can be used either with the api or it can produce a file to be uploaded. To use the api, use the `-a` flag. To produce an rdf file, use the `-r` flag. You also must include the path to a yaml config file.

`python hermes.py -a config.yaml`

## Config
There are several required entries in your config file.
*email*
The user account for your VIVO account. If you are using the api option, this account will most likely need admin rights.

*password*
The password to your VIVO account.

*update_endpoint*
The url for the update endpoint. If you are not using the api, this can be blank.
*query_endpoint*
The url for the query endpoint.

*namespace*
The namespace for the uris on your VIVO instance.

*folder_for_logs*
The folder to put Errol's logs in.

*filter_folder*
The folder containing filters for cleaning up the names and titles of entities.