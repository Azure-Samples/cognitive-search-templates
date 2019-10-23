---
page_type: sample
languages:
  - Power BI Template
products:
  - azure
  - azure-search
name: Power BI template for knowledge store
description: 'A Power BI template with visualizations intended for knowledge stores created using the Import data wizard in the Azure portal.'
urlFragment: "/powerbi/templates"
---

# Power BI template for knowledge store (Azure Search)

![Flask sample MIT license badge](https://img.shields.io/badge/license-MIT-green.svg)

This repository contains a Power BI template that provides visualzations for a [knowledge store created by the Import data wizard](https://docs.microsoft.com/azure/search/knowledge-store-create-portal) in the Azure portal. 

When creating a knowledge store through the wizard, you have the option of downloading a Power BI template. Choosing that option brings you to this repository so that you can download the file. 

Alongside the download link, the wizard gives you the parameters you'll need to initialize the dashboard from your desktop. Copy those parameters from the wizard now and save them for when you want to run the dashboard.

## Contents

This repository contains the following items.

| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `powerbi/`        | Folder containing the sample Power BI template.|
| `.gitignore`      | Define what to ignore at commit time.      |
| `CONTRIBUTING.md` | Guidelines for contributing to this project. |
| `SECURITY.md`     | Instructions for reporting security bugs. |
| `README.md`       | This README file.                          |
| `LICENSE`         | The license for the sample.                |


## Prerequisites

1. You must have Power BI Desktop to use the template.

1. For Azure Search, you must have filled in the second page of the Import data wizard in the Azure portal to create the knowledge store. The second page of the wizard captures the following inputs, which are necessary for using the Power BI template.

   + Include cognitive skills in the import process (this creates the skillset)
   + Include the save to knowledge store option (this creates the knowledge store)
   + Include projection options that save enriched content to tables (this structures the knowledge store)

1. The wizard must have created all objects and enrichments before you can run the report. You can verify the knowledge store exists by using [Storage Explorer in the Azure portal](https://docs.microsoft.com/azure/search/knowledge-store-view-storage-explorer) to examine the table projections in Azure Table storage.

1. Requirements for using the dashboard include the following parameters, which you can obtain from the wizard or the Azure portal:

   + Skillset name
   + Source data field (the field you chose to enrich, often it's `content` or `merged_content`)
   + Enrichment granularity (Document, Pages, Sentences)
   + Storage account used for knowledge store

## Set up the dashboard

You must have finished running the wizard, and all objects must exist. The knowledge store must contain the enriched content.

1. Click the repository name **cognitive-search-templates** to go to the root folder.
1. Click **Clone or Download** to get the file. If you download a zip file, right-click to extract its contents.
1. Start Power BI Desktop.
1. On File > Import > Power BI Templates, choose the **cognitive-search-content-analytics-template.pbit** file.
1. When prompted, provide the following parameters:
   +  Skillset name
   +  Source data field
   +  Enrichment granularity (document, page or sentence)
   +  Knowledge store (storage) account name

On first use, you will be prompted for the Storge account access key.

## Runnning the sample

Once you have the data loaded from Azure tables into Power BI, you can explore latent relationships, hierarchy, and the structure of enriched content. 

## Key concepts

This is an example of a Power BI template. It includes visualizations that tend to work well with enriched content. You can use this example as-is, or adapt it to accommodate more complex skillsets or projections.
