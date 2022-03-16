# Sbd4Nano Landscape

This repository relates to SbD4Nano Task 2.1.1 "Library of comprehensive data on ENMs properties and bioactivities".

## Plan

* create turtle files with metadata info of datasets, databases, models and data sources of safety knowledge
* keep manually added data in a separate files
* we'll extract automatically data and models from:
   * Data sets
      * FAIRSharing (API) (open data)
      * Wikidata (SPARQL) (open data)
      * NanoWiki (Studies, RelationShips): https://github.com/h2020-sbd4nano/sbd-data-aopwiki (private repo)
      * AOPWiki: https://github.com/h2020-sbd4nano/sbd-data-aopwiki (private repo)
      * Diamonds spreadsheet: https://github.com/h2020-sbd4nano/sbd-data-diamonds/  (private repo)
   * Models
      * JRC
      * QSARDB
      * NanoSolveIT / NanoInformaTIX
   * SbD4Nano
      * Deliverable D4.1
      * Deliverable D1.1
* develop a SPARQL endpoint with SNORQL interface

## What questions should the knowledgebase

### Give me all datasets, bases, and models

* with a license that allows integration in the SbD4nano platform
* which tell me about NOEL, DNEL, or PNEC for a particular nanomaterial
* what is all knowledge about the safety of a partcular nanomaterial

## Database validation

### Turtle syntax

The Turtle content can be validated according to the syntax with:

```shell
cat nanosafety_databases.ttl | rapper -i turtle -t -q - . > /dev/null
```

### Shape Expression validation

The Turtle content is also validated against shape expressions written
in the ShEx standards. These can be found in the [shapes/](shapes/) folder.

## Analysis

We use SPARQL to summarize and visualize the collected data.

## License information for data

License information for data in this folder is provided in the VoID header
files for that data.
