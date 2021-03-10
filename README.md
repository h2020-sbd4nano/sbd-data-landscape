# Sbd4Nano Dataset / Database Landscape

THIS REPO IS PRIVATE AND UNTIL WE HAVE PERMISSION MUST NOT BE SHARED.

This repository relates to SbD4Nano Task 2.1.1 "Library of comprehensive data on ENMs properties and bioactivities".

## Plan

* create turtle files with metadata info of datasets and databases
  * model *everything* for now as `void:Dataset`
* keep manually added data in a separate file
* we'll extract automatically data and models from:
   * Data sets
      * FAIRSharing (API)
      * Wikidata (SPARQL)
      * NanoWiki (Studies, RelationShips): https://github.com/h2020-sbd4nano/sbd-data-aopwiki
      * AOPWiki: https://github.com/h2020-sbd4nano/sbd-data-aopwiki
      * WP1 spreadsheet
      * Diamonds spreadsheet: https://github.com/h2020-sbd4nano/sbd-data-diamonds/blob/main/diamonds-models.ttl 
   * Models
      * JRC (?)
      * QSARDB (?)
      * NanoSolveIT / NanoInformaTIX (?)
   * SbD4Nano
      * Deliverable D4.1
      
NB. Information about Diamonds models with an unknown license can be found [in this repository](https://github.com/h2020-sbd4nano/sbd-data-diamonds/)

## Database validation

### Turtle syntax

The Turtle content can be validated according to the syntax with:

```shell
cat nanosafety_databases.ttl | rapper -i turtle -t -q - . > /dev/null
```

## Analysis

We will use SPARQL to summarize and visualize the collected data.
  
## License
  
Data collected in the repository has multiple licenses. E.g. data from Wikidata is CC0.
If not otherwise specified, the data in this databases is CC0.
  
 
