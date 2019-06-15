# Blackbird-2019

A fork of the **darkarnium/kako** project, Blackbird-2019 is an extension of the kako framework, that utilizes the JSON data it creates for data analysis and cybersecurity research. Kako is capable of virtualizing and deploying embedded devices with security vulnerabilities to act as low-interaction honeypots. Data is then created from foreign entities interacting with these honeypot instances and saved for future analysis. 

While kako has its own method for performing data analysis on AWS SNS, Blackbird's goal is to be able to act as an semi-automated system that can analyze payloads remotely via the SHODAN/Search API in order to differentiate between neutral to suspicious/hostile activity by possible attackers. Jupyter Notebook is used as a front-end to analyze data with preloaded numpy/pandas code set to analyze received data, and even geolocate the origin of some connections with a real-time map module. 

As Blackbird-2019 is in its early stages of development, several features planned for it, such as an IDS/IPs system and threat domain lookup will be implemented in the near future.

## Dependencies

The following Python packages are required for the Kako and Blackbird-2019 framework to function correctly:

* `click` - Command-line argument processing.
* `boto3` - Amazon AWS integration.
* `requests` - HTTP request library.
* `cerberus` - Validation of messages and other documents.
* `jupyter-notebook` - Front-end GUI for data analysis

Once these modules are installed, a valid configuration file is required. See the **Configuration** section for more information.

## Usage

Usage of Kako commands require the following: ``kako-master --configuration-file PATH_TO_KAKO_YAML --simulation-path PATH_TO_SIMULATION_YAMLs``

Kako's innate extensibility allows for additional services to be utilized by modifying or creating new .yaml files in the simulation folder during setup.

## Additional Reading

* Example and common Kako 
    * https://www.github.com/darkarnium/kako
* Example and common Kako simulations
    * https://www.github.com/darkarnium/kako-simulations/
* Ogawa project for consuming data from AWS SQS into ElasticSearch.
    * https://www.github.com/darkarnium/ogawa/
