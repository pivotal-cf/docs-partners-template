This repo currently includes templates for the following topics:

* [index.html.md.erb](./docs-content/index.html.md.erb): The index of your docs.
* [installing.html.md.erb](./docs-content/installing.html.md.erb): How to install and configure your product tile.
* [using.html.md.erb](./docs-content/using.html.md.erb): How to use your product.
* [release-notes.html.md.erb](./docs-content/release-notes.html.md.erb): Release notes for your product.

To begin using this repo to develop your documentation, perform the following steps:

1. Make a fork of this repo.
1. Clone your fork onto your local machine.
1. Work your way through each topic, replacing the placeholders in ALL-CAPS and following the instructions in **bold**. 
    * When writing your documentation, follow the guidelines in [Style Notes for Tile Authors](style-guide.md).
1. Complete the subnav by replacing the placeholders in ALL-CAPS in the subnav file at `docs-book/master_middleman/source/subnavs/myservice_subnav.erb` in this repo.
1. When you've finished your documentation, make a pull request to merge your fork into this repo and email the ISV team at ISV-TPM@pivotal.io.

### About Subnavs of Published Tile Documentation

After your tile documentation has been published, the subnav used for the live documentation is contained in this directory: https://github.com/pivotal-cf/docs-book-partners/tree/master/master_middleman/source/subnavs

However, you should also continue to maintain the local subnav file.

To edit a subnav for your tile documentation, follow these steps:

1. Make a pull request against the subnav file in https://github.com/pivotal-cf/docs-book-partners/tree/master/master_middleman/source/subnavs

2. Make the same changes in the subnav file (in /docs-book/master_middleman/source/subnavs/ of your tile repo) and make a pull request for that change too.

Happy documenting!
