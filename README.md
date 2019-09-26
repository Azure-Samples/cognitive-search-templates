---
page_type: sample
languages:
- Power BI Template
products:
- Azure Cognitive Search
description: "templatefor visualizing your enriched data from the knowledge store."
urlFragment: "/powerbi/templates"
---

# Official Microsoft Sample

This repository contains the samples to jump start your knowledge mining experience. Starting with a Power BI template that works out of the box with knowledge store projections, created with the import data workflow in the Azure Cognitive Search service.

## Contents

Outline the file contents of the repository. It helps users navigate the codebase, build configuration and any related assets.

| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `src`             | Sample source code.                        |
| `.gitignore`      | Define what to ignore at commit time.      |
| `CHANGELOG.md`    | List of changes to the sample.             |
| `CONTRIBUTING.md` | Guidelines for contributing to the sample. |
| `README.md`       | This README file.                          |
| `LICENSE`         | The license for the sample.                |
| `powerbi/`        | Folder conatining the sample Power BI template.|

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
3. Enrichment granularity 
4. Knowledge store (storage) account name
5. You will be prompted for the storge account key the first time

## Runnning the sample

Once you have the data loaded from tables into Power BI, you can now explore your enriched data with Power BI!

Explore latent relationships, hierarchy and the structure you created with the enrichments. 

## Key concepts

This is an example of a Power BI template that you can build based on your enriched data. As you build more complex skillsets, edit your projections, you can then edit this template or create a new one to explore the enrichments.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
