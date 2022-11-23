# gwasdiversity_by_funder

A repository to build a prototype of new functionality for the GWAS Diversity Monitor.

This readme.md is designed to document things that I think need further discussion or review within the repo/the broader body of work.

1. Do we want the search functionality to be via Agency or via Acronym? I believe this should be 'Agency'.
2. However, we're going to need to clean the Agency field quite substantially.
   1. Work still needs to be done to clean duplicates (i.e. the same identical funder being identified via multiple string identifiers).
   2. How do we group broader agencies together? For example, should we group all the NIH sub-agencies? TBC 
3. Do we still want to keep Associations for the doughnut, even if it only filters for the initial stage?
4. As part of the new generate_data.py, we have a _substantial_ number of 'null' occurances where funders arent funding anything in specific years. How this is going to be handled requires further discussion.
5. The sumstats dictionary (`sumarry.json`) now has an additional key to delineate by funder. This needs to be integrated into new frontend work.
