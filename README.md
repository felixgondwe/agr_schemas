[![Build Status](https://travis-ci.org/alliance-genome/agr_schemas.svg?branch=development)](https://travis-ci.org/alliance-genome/agr_schemas)

AGR JSON Schemas
================

This directory contains JSON schemas used to define data for integration into AGR.

Most recent release:

|Schema|Description|
|---------|----------|
|basicGeneInfoFile|A file of Basic Gene Information objects. This is the base or "root" schema.|
|basicGeneInformation|An entry with Gene information from a MOD.  Gene set includes: genes, psuedogenes and not-protein coding genes.  It does not include engineered foreign genes, transcripts or other features.|
|dataProvider|An standard set of information regarding data source and taxon ids for the AGR.|
|crossReference|An crossReference entity (_e.g._: NCBIGENE links, UniProt Links, and links back to MODs).
|metaData|An standard set of information regarding when and from whom the load was generated.|

Validation
----------
The python script "agr_validate.py" can be used to validate a JSON entry against a schema for testing/development purposes.
Usage is as follows: 
`agr_validate.py -d test_data.json -s base_schema.json`

Formatting Notes
----------------
Please use 2 spaces for indentation.
