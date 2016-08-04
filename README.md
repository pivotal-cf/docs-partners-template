## Pivotal Cloud Foundry Partners Template

This template helps partners prepare documentation for Pivotal Cloud Foundry (PCF) partner services that appear on [Pivotal Network](https://network.pivotal.io/). 

### <a id='overview'></a>Overview

Every partner service in PCF is documented on our PCF documentation site. The links to these partner service docs appear on the [front page](http://docs.pivotal.io) under **Partner Services for Pivotal Cloud Foundry**.

For a good example of a partner service doc, see [ISS Knowtify Search Analytics](http://docs.pivotal.io/knowtify/index.html).

### <a id='template'></a>How To Use This Template

Partners use this template to develop the documentation for their PCF service. This repo currently includes templates for the following topics:

* [index.html.md.erb](index.html.md.erb): The index of your docs.
* [installing.html.md.erb](installing.html.md.erb): How to install and configure your product tile.
* [using.html.md.erb](using.html.md.erb): How to use your product.
* [release-notes.html.md.erb](release-notes.html.md.erb): Release notes for your product.

To begin using this repo to develop your documentation, perform the following steps:

1. Clone this repo onto your local machine.
1. Work your way through each topic, replacing the placeholders in ALL-CAPS and following the instructions in **bold**. 
1. Complete the subnav by replacing the placeholders in ALL-CAPS in the subnav file at `docs-book/master_middleman/source/subnavs/myservice_subnav.erb` in this repo.
1. View your documentation as a live local site in a browser, by following the steps below in the [How To Use Bookbinder To View Your Docs](#bookbinder) section.
1. When you've finished your documentation, push your docs up to the remote and email the PCF Docs Team at cf-docs@pivotal.io.

### <a id='bookbinder'></a>How To Use Bookbinder To View Your Docs

[Bookbinder](https://github.com/pivotal-cf/bookbinder/blob/master/README.md) is a command-line utility for stitching Markdown docs into a hostable web app. The PCF Docs Team uses Bookbinder to publish our docs site, but you can also use Bookbinder to view a live version of your documentation on your local machine.

Bookbinder draws the content for the site from `docs-content`, the subnav from `docs-book`, and various layout configuration and assets from `docs-layout`.

To use Bookbinder to view your documentation, perform the following steps:

1. On your local machine, `cd` into `docs-book` in the cloned repo.
1. Run `bundle install` to make sure you have all the necessary gems installed.
1. Build your documentation site with `bookbinder` in one of the two following ways:
	* Run `bookbinder watch` to build an interactive version of the docs and navigate to `localhost:4567/myservice/` in a browser. (It may take a moment for the site to load at first.) This builds a site from your content repo at `docs-content`, and then watches that repo to update the site if you make any changes to the repo.
	* Run `bookbinder bind local` to build a Rack web-app of the book. After the bind has completed, `cd` into the `final_app` directory and run `rackup`. Then navigate to `localhost:9292/myservice/` in a browser.
