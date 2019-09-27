## Prerequisites

You will need to setup an enrichment pipeline within Azure Cognitive Search with the following options:
1. Select the knowledge store option
2. Project your enrichments to tables

As you go throught the process, saving the following bits of information will help you in the following steps:
1. The skillset name
2. Source data field (the field you chose to enrich)
3. Knowledge store storage account name

## Setup

Once you have a knowledge store populated with enriched data in tables, download the template file, open it in Power BI, you will be prompted for the following:
1. Skillset name
2. Source data field
3. Enrichment granularity (document, page or sentence)
4. Knowledge store (storage) account name
5. You will be prompted for the storge account key the first time

## Runnning the sample

Once you have the data loaded from tables into Power BI, you can now explore your enriched data with Power BI!

Explore latent relationships, hierarchy and the structure you created with the enrichments. 

## Key concepts

This is an example of a Power BI template that you can build based on your enriched data. As you build more complex skillsets, edit your projections, you can then edit this template or create a new one to explore the enrichments.
