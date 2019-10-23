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

# Power BI template for knowledge store

![Flask sample MIT license badge](https://img.shields.io/badge/license-MIT-green.svg)

This repository contains a Power BI template that provides visualzations for a [knowledge store created by the Import data wizard]() in the Azure portal. 

When you create a knowledge store through the wizard, you have the option of downloading a Power BI template. Choosing that option brings you to this repository so that you can download the file. 

Alongside the download link, the wizard gives you the parameters you'll need to initialize the dashboard from your desktop. Copy those parameters from the wizard now and save them for when you want to run the dashboard.

## Contents

This repository contains the following items.

| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `powerbi/`        | Folder conatining the sample Power BI template.|
| `.gitignore`      | Define what to ignore at commit time.      |
| `CONTRIBUTING.md` | Guidelines for contributing to this project. |
| `SECURITY.md`     | Instructions for reporting security bugs. |
| `README.md`       | This README file.                          |
| `LICENSE`         | The license for the sample.                |


## Prerequisites

1. You must have Power BI Desktop to use the template.

1. For Azure Search, you must have used the Import data wizard in the Azure portal, and the wizard must have captured the following inputs. These inputs are specified on the second page of the wizard.

   + Include cognitive skills in the import process
   + Include the save to knowledge store option
   + Include projection options that save enriched content to tables

1. The wizard must be finished, having created all objects and enrichments, before you can run the report. You can verify the knowledge store exists by using Storage Explorer in the Azure portal to examine the table projections in Azure Table storage.

1. Dashboard Later, after you download the template, you'll need to enter the following information to initialize the dashboard, which you can obtain from the wizard or the Azure portal:

+  Skillset name
+  Source data field (the field you chose to enrich, often it's `content` or `merged_content`)
+  Enrichment granularity (Document, Pages, Sentences)
+  Storage account used for knowledge store

## Set up the dashboard

Bou must have finished running the wizard, with all objects and the knowledge store created.
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

Once you have the data loaded from tables into Power BI, you can now explore your enriched data with Power BI.

Explore latent relationships, hierarchy, and the structure you created with the enrichments. 

## Key concepts

This is an example of a Power BI template that you can build based on your enriched data. As you build more complex skillsets, edit your projections, you can then edit this template or create a new one to explore the enrichments.
