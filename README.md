# CAP Organ List Ontology

A repository for building organ list for the Cell Annotation Platform.

## General Work FLow

- Make robot template to generate cap_organ_subset tags for this list of terms. Build to test.
- Robot template will live in new repo 
- Add to triplestore loading config (GitHub raw URL) : https://github.com/kharchenkolab/cap-pipeline-config/blob/main/config/collectdata/vfb_fullontologies.txt
- Update the script that updates the YAML config to point to our local knowledgeBase
- Update the organ SPARQL query to use this new subset


## Prerequisite

ROBOT is a tool for working with Open Biomedical Ontologies. It can be used as a command-line tool or as a library for any language on the Java Virtual Machine. For installation please see http://robot.obolibrary.org.


## Building

1. Go into ontology folder under src directory
    ```
    cd src/ontology
    ```

2. Run the Makefile with following command to produce the cap_organ_slim.owl under src/results directory
    ```
    make all
    ```
