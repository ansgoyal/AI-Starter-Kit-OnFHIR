# Chapter 1 - Synthea: Generate FHIR patient and financial bundles

#### This chapter shows how to setup and generate health records with Synthea.

Synthea is an open-source synthetic patient and associated health records generator that simulates the medical history of synthetic patients.
Synthea generates HL7 FHIR records using the HAPI FHIR library to generate a FHIR Bundle for [these](https://github.com/synthetichealth/synthea/wiki/HL7-FHIR) FHIR Resources.
More on Synthea [here](https://github.com/synthetichealth/synthea).

By default, Synthea contains publicly available demographic data obtained from the US Census Bureau. The data was post-processed to create population input data for every place (town and city) in the United States. This post-processed data can be used with Synthea to generate representative populations. (County + SubCounty + Education + Income)

## Prerequisites
* Java 1.8 (select JDK, not JRE install)

## Setup Synthea
* Follow the [setup](https://github.com/synthetichealth/synthea/wiki/Basic-Setup-and-Running) instructions and download the .jar file.
* Copy [synthea.properties](./synthea.properties) file to the same location as the .jar file downloaded above.
* Run the jar file with the parameters. Example: java -jar synthea-with-dependencies.jar -s 1048576 -p 100 Texas -c <path>\synthea.properties . More examples in the link above.
* Output json files will be saved in output folder in the same directory.

***

[Go to Chapter 2 - Azure API for FHIR: Create and configure](../Chapter2-AzureAPIforFHIR/ReadMe.md)
