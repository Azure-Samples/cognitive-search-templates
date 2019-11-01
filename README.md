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

# Power BI sample template for knowledge store (Azure Search)

![Flask sample MIT license badge](https://img.shields.io/badge/license-MIT-green.svg)

This repository contains a Power BI template that provides visualizations for a [knowledge store created by the Import data wizard](https://docs.microsoft.com/azure/search/knowledge-store-create-portal) in the Azure portal. 

In the **Import data** wizard, next to the template download link, look for and save the following values:
  + Skillset name
  + Content field
  + Enrichment granularity
  + Storage account

These values are required by the sample template.

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

+ [Power BI Desktop](https://powerbi.microsoft.com/downloads/)

+ A knowledge store created in the Azure Portal with the **Import data** wizard. To create a knowledge store, in the **Import data** wizard, on the **Add cognitive search page** (second page in the wizard), fill out all sections including:

   + **Add enrichments**: These options create the skillset based on the skills you select.
   + **Save enrichments to a knowledge store**: These options create the knowledge store. You must select **Azure table projections** to save the enriched content to tables. This wizard section also contains a link to this repository and shows values that will be required to initialize the template: skillset name, content field, enrichment granularity, and storage account. Copy and save these values.

  After you complete the **Import data** wizard, wait for the knowledge store to be populated with the enriched content before you open the sample template. To verify that the knowledge store content is available, use the [Storage Explorer in the Azure portal](https://docs.microsoft.com/azure/search/knowledge-store-view-storage-explorer) to view the table projections in the Azure storage account.

## Download the sample template

In this repository, go to the [**cognitive-search-templates**](https://github.com/Azure-Samples/cognitive-search-templates) folder and click  **Clone or Download** to clone the repository or download a ZIP file. If you download a ZIP file, right-click the file to extract its contents.

## Connect the Power BI template with your knowledge store

1. Start Power BI Desktop.
1. Go to **File** > **Import** > **Power BI Template**, and select the _cognitive-search-content-analytics-template.pbit_ file.
1. When prompted, provide the following parameters:

   + Skillset name
   + Source data field (content field): This is the field you chose to enrich. It is often named _content_ or _merged_content_.
   + Enrichment granularity level (document, pages, or sentences)
   + Knowledge store storage account name

   These are the values you saved during the **Import data** wizard process.

   On first use, you may also be prompted for the storage account access key.

## Analyze your data with Power BI visualizations

Once you have the data loaded from Azure tables into Power BI, you can explore the latent relationships, hierarchy, and structure of your enriched content.

## Key concepts

This is an example of a Power BI template. It includes visualizations that tend to work well with enriched content. You can use this example as-is, or adapt it to accommodate more complex skillsets or projections.
