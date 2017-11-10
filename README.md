# HXS (Humanitarian Exchange Server)
![HXS Diagram](https://github.com/HXS-API/Server/blob/master/hxs_server.png)
HXS is an open source initiative bringing humanitarian organizations, tech volunteers and supporters together to setup an enterprise-grade IATI database, server and API for developers to use to prototype, test power and scale next-generation, IATI-data-driven applications.

## Function

**IATI** is a technical framework managed by the [International Aid Transparency Initiative](http://iatistandard.org) that the humanitarian community has been working concertedly to setup and broadly mandate. The framework provides organizations and donors with a channel to openly share and compare detailed information on aid activities, transactions and results and make the information accessible to machine applications.

However, IATI's [datastore](http://datastore.iatistandard.org/docs/) and [API](https://iatiregistry.org/registry-api) aren't adapted to dedicatedly power modern, enterprise-grade applications. So we're building an IATI data source that is sophisticated and robust enough to address the need.

## Architecture

HXS is being built using AWS components. HXS's Python [codebase]() will principally run from within an EC2 instance and carry out four main operations:

* Identify the URL locations of all known IATI files by scraping the IATI Registry
* Strip XML file information from each URL and generate a single XML file
* Process the XML file and database information on aid activities
* Automate the operations, checking IATI daily to maintain a fully up-to-date IATI dataset

### Output

The Humanitarian Exchange Server will give developers full access to IATI’s entire dataset and the ability to carry out sophisticated operations, querying the dataset in a host of ways employing any of IATI’s 217 plus information fields (counted by XPath).

The server will also give developers the ability to use HXS’s IATI clone like a cloud database, giving applications the ability to read and carry out write, update and delete operations enabling users to start, edit, share and compare IATI compliant files before formally publishing their files to IATI.

## Get involved

We can use help to setup HXS’s AWS architecture, develop and test HXS’s codebase and produce some API documentation as well as a help to test and improve the Humanitarian Exchange Server and setup a basic HXS.ngo landing page website. To get involved or to learn more about the project, **contact**: hxs(at)beehive.ngo
