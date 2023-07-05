# A SKOS vocabulary for the catalysis disciplines

> **The first collection of terms has just been made public (June-2023)**.
> **We will add more content in the coming weeks and month.**

The vocabulary has been created and maintained as part of the [NFDI4Cat](http://www.nfdi4cat.org) initiative and follows our [Voc4Cat Guidelines](https://doi.org/10.5281/zenodo.7669183).

This repository was created from the template [voc4cat-template](https://github.com/nfdi4cat/voc4cat-template).
It uses the [voc4cat-tool](https://github.com/nfdi4cat/voc4cat-tool) and GitHub features like gh-actions, pull requests etc. to reduce the maintenance workload for contributors and editors.

## Basic principles

All vocabularies managed here have the same standard contribution process,

- get and update the vocablary file (xlsx),
- submit a pull request with the updated file,
- collaborate on the pull request with editors or other github users,
- approval and merge of the pull request.

Finally the SKOS-vocabularies land in the folder `vocabularies` in turtle-format.

In addition, documentation is created automatically and published on github-pages.

- The general url is `https://{gh-org-name}.github.io/{vocabulary-name}/docs/`
- In repository `nfdi4cat/voc4cat` the vocabulary `vocab_example` is documented at [https://nfdi4cat.github.io/voc4cat/voc4cat/](https://nfdi4cat.github.io/voc4cat/voc4cat/)

## Contributing to vocabularies

To discuss about the SKOS-vocabularies maintained here, create an [issue](https://github.com/nfdi4cat/voc4cat/issues).

To contribute new concepts or collections or change existing ones, you may either submit your contributions as Excel-file or (as an expert) as new/changed turtle file.

> *To try out the workflow with some example data, you may use  [voc4cat-playground](https://github.com/nfdi4cat/voc4cat-playground) which is identical to this repository but will be purged from time to time.*

Here are the steps for submitting updates in Excel.

- Get the Excel-vocabulary file
  - For an existing vocabulary, the latest version of the vocabulary is always available via github-pages.
    - The general url is `https://{gh-org-name}.github.io/{vocabulary-name}/{vocabulary-name}.xlsx`
    - For example here the vocabulary `vocab_example` can be downloaded from [https://nfdi4cat.github.io/voc4cat/vocab_example.xlsx](https://nfdi4cat.github.io/voc4cat/vocab_example.xlsx)
  - For setting up a new vocabulary, use the xlsx-file from the templates-folder.
- Make changes to the Excel file
- Add the Excel file to your clone of the repository into the folder `inbox-excel-vocabs`
  - The name of the Excel-file must match the vocabulary that you want to update (e.g. myvoc.xlsx to update a vocabulary named "myvoc").
  - New vocabularies will be named like the Excel-file (minus the .xlsx-extension).
- Create a pull request with the updated Excel-file on github.
  - Please describe your changes and the motivation for the changes in the pull request note or link to an issue with this information. This will help reviewers to understand the proposed change and decide about it.
- Your pull request will be processed automatically by a CI/CD pipeline that typically runs less than a minute.
- Review the artifacts/logs generated by the CI pipeline.
- If all is good your contribution will be either
  - directly merged by the maintainers
  - or a discussion will be started about what else is needed
  - or why the proposed change may not fit.
- If you need to fix something just update the pull request branch. This will trigger the pipeline to run again.

Finally, when the proposed merge request is accepted, your changes will be integrated in the vocabularies in the folder [vocabularies](https://github.com/nfdi4cat/voc4cat/tree/main/vocabularies).

See [inbox-excel-vocabs/README.md](inbox-excel-vocabs/README.md) for a minimal example how to test the submission process.

## How to suggest improvements to the tooling & template?

To discuss about the workflow for maintaining SKOS vocabularies based on this template, create an [voc4cat-template issue](https://github.com/nfdi4cat/voc4cat-template/issues).

To discuss about the tool that converts Excel to SKOS in gh-actions of this template, create an [voc4cat-tool issue](https://github.com/nfdi4cat/voc4cat-tool/issues).

## Authors and acknowledgment

### Vocabularies

- *List all contributors.*

### Voc4cat template

- David Linke (ORCID: 0000-0002-5898-1820) - Initial setup of repository and CI/CD pipelines

## License

### Vocabularies

All vocabularies in this repository are CC0 licensed, see [LICENSE](LICENSE) for details.

### Voc4cat template

The template itself is CC0 licensed, see [LICENSE](LICENSE). Although there is no obligation, we nevertheless appreciate if our work is acknowledged in any derivative work.

## Acknowledgement

This work was funded by the German Research Foundation (DFG) through the project "[NFDI4Cat](https://www.nfdi4cat.org) - NFDI for Catalysis-Related Sciences" (DFG project no. [441926934](https://gepris.dfg.de/gepris/projekt/441926934)), within the National Research Data Infrastructure ([NFDI](https://www.nfdi.de)) programme of the Joint Science Conference (GWK).
