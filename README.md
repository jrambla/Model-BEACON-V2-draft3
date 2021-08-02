# beacon-v2-Models: The Beacon v2 draft 3 Model
This repo hosts the Beacon v2 draft 3 model for reference purposes, as it has been the active one for many months in the Beacon project and many documents, example code and presentations refers to this version.

+++++ IT MUST BE CONSIDERED FROZEN +++++

## Introduction
The GA4GH Beacon specification is composed by two parts:

* the Beacon Framework
* the Beacon Models

The **Beacon Framework** (in [Framework repo](https://github.com/ga4gh-beacon/beacon-framework-v2) repo) is the part that describes the overall structure of the API requests, responses, parameters, teh common components, etc. It could also be referred in this document as simply the *Framework*.

**Beacon Models** describes the set of concepts included in a Beacon version (e.g. Beacon v2), like *individual* or *biosample*, and also the relationships between them. It could also be referred in this document as simply the *Model*. 

The Framework could be considered the *syntax* and the Model as the *semantics*. 

Refer to the [Framework repo](https://github.com/ga4gh-beacon/beacon-framework-v2) for further information about the Framework and its parts.

A **Beacon instance** is just an implementation of a Beacon Model that follows the rules stated by the Beacon Framework.

If you are a Beacon implementer, then, you don't need to clone the Framework repo, you only need to **copy** (*or clone*) a Beacon Model and modify it to your specific case. You will find plenty of references to the Framework in the Model copy, and you will use the Json schemas there to validate that both the structure of your requests and responses are compliant with the Beacon Framework. The Framewrok is not used to check the schema in the responses payload (e.g. the actual details of a biosample of a cohort). The schemas for that are included in the Model that you should have copied.

Refer to the [Models repo](https://github.com/ga4gh-beacon/beacon-v2-Models) for a list of other Models.