# Blackbird-2019

A fork of the **darkarnium/kako** project, Blackbird-2019 is an extension of the kako framework, that utilizes the JSON data it creates for data analysis and cybersecurity research.

This project provides honeypots for a number of well known and deployed embedded device vulnerabilities.

This project is intended for use in cataloging attack sources, droppers and payloads. The default configuration will run a given set of simulations and capture information relating to the origin of the requests, the body of the request, and attempt to process and collect the payload - if supported.

## Dependencies

The following Python packages are required for Kako to function correctly:

* `click` - Command-line argument processing.
* `boto3` - Amazon AWS integration.
* `requests` - HTTP request library.
* `cerberus` - Validation of messages and other documents.

Once these modules are installed, a valid configuration file is required. See the **Configuration** section for more information.

## Additional Reading

* Example and common Kako simulations
    * https://www.github.com/darkarnium/kako-simulations/
* Ogawa project for consuming data from AWS SQS into ElasticSearch.
    * https://www.github.com/darkarnium/ogawa/
