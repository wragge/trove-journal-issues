# Trove journal issues

This repository contains a series of CSV files that capture information about digitised journals available on Trove. There is one CSV file per journal. Each file contains a list of available issues. The files were created [using this notebook](https://glam-workbench.net/trove-journals/get-ocrd-text-from-all-journals/) in the GLAM Workbench.

Each CSV file includes the following fields:

* `title` – title of the journal
* `id` – Trove's identifier for the journal
* `details` – publication details of this issue, usually volume/issue numbers and dates
* `pages` – number of pages in the issue
* `text_file` – name of the file containing the full text of this issue

To browse the list of journals (with links to CSV files and full text downloads) [go to the GLAM Workbench](https://glam-workbench.net/trove-journals/journals-with-ocr/). A [machine-readable list of journals with OCRd text](https://glam-workbench.net/trove-journals/csv-journals-with-ocr/) is also available.

The full text contents of each journal issue has been downloaded from Trove and saved in a `zip` file. The `zip` files can be downloaded from an s3 bucket, either using [this human-readable list](https://glam-workbench.net/trove-journals/journals-with-ocr/), or by constructing a url [using this CSV file](https://glam-workbench.net/trove-journals/csv-journals-with-ocr/). Just insert the contents of the `directory` field into a url of the form `https://trove-journals.s3.ap-southeast-2.amazonaws.com/[directory value].zip`. For example: <https://trove-journals.s3.ap-southeast-2.amazonaws.com/14th-company-magazine-nla.obj-15956697.zip>