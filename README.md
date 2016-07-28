## Pivotal Cloud Foundry Partners Template

This repo helps partners prepare documentation for Pivotal Cloud Foundry (PCF) partner services that appear on [Pivotal Network](https://network.pivotal.io/). 

### <a id='overview'></a>Overview

Every partner service in PCF is documented on our PCF documentation site. The links to these partner service docs appear on the [front page](http://docs.pivotal.io) under **Partner Services for Pivotal Cloud Foundry**.

For a good example of a partner service doc, see [ISS Knowtify Search Analytics](http://docs.pivotal.io/knowtify/index.html).

### <a id='template'></a>How To Use This Template

Partners use this repo to develop the documentation for their PCF service. This repo includes templates for the following topics:

	* [index.html.md.erb](index.html.md.erb): The index of your docs.
	* [installing.html.md.erb](installing.html.md.erb): How to install and configure your product tile.
	* [using.html.md.erb](using.html.md.erb): How to use your product.
	* [release-notes.html.md.erb](release-notes.html.md.erb): Release notes for your product.

To begin using this repo to develop your documentation, perform the follow steps:

	1. Fork this repo.
	1. Work your way through each topic, replacing the placeholders in ALL-CAPS and following the instructions in **bold**. To view your documentation as a live local site in a browser, follow the steps below in the [How To Use Bookbinder To View Your Docs](#bookbinder) section.
	1. When you're done, email the link to your branch to the PCF Docs Team at cf-docs@pivotal.io.

### <a id='bookbinder'></a>How To Use Bookbinder To View Your Docs

Bookbinder is a command-line utility for stitching Markdown docs into a hostable web app. The PCF Docs Team uses Bookbinder to publish our docs site, but you can also use Bookbinder to view a live version of your documentation on your local machine.

### <a id='publish'></a>How We Publish Your Docs

When we receive your documentation, we will review it and create a repo for it in our `pivotal-cf` GitHub organization. When your product is published on Pivotal Network, we will add the link to your documentation on the front page of the PCF docs site.

### <a id='changes'></a>How To Make Changes To Your Docs In The Future

We will provide you with the name of the repo where your docs live, so that if you want to make changes in the future, you can submit a PR against it. Or, if you have bigger changes and want to collaborate on drafting the documentation, feel free to email us at cf-docs@pivotal.io. We’re always happy to help! 

