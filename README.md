# HXS (Humanitarian Exchange Server)
![HXS Diagram](https://github.com/HXS-API/Server/blob/master/HXS_API.png)
HXS is an open source initiative launched by [Beehive](https://beehive.ngo) volunteers that's bringing humanitarian organizations, tech volunteers and supporters together to setup an **enterprise-grade IATI database**, **server** and **API** for developers to use to prototype and scale next-generation IATI-data-driven applications.
## Function

**IATI** is a technical framework managed by the [International Aid Transparency Initiative](http://iatistandard.org) that the humanitarian community has been working concertedly to setup and broadly mandate. The framework provides organizations and donors with a channel to openly share detailed information on aid activities, transactions and results and make the information accessible to machine applications.

However, IATI's [datastore](http://datastore.iatistandard.org/docs/) and [API](https://iatiregistry.org/registry-api) aren't adapted to dedicatedly power modern, enterprise-grade applications. So we're building an IATI data server and API that are sophisticated and robust enough to address the need.

## Architecture

The Humanitarian Exchange Server is being built using AWS components and its Python [codebase](https://github.com/HXS-API/Server/tree/master/Codebase) will principally run from within an EC2 instance and carry out four main operations:

* Identify the URL’s of organizations’ IATI XML files by scraping the IATI registry
* Strip organizations’ IATI files and combine file information into one master XML file
* Process the master file and database any new and updated IATI information
* Automate the operations, checking IATI regularly to maintain an up-to-date copy of IATI's entire dataset

### API

The Humanitarian Exchange Server’s API will give registered developers with user keys the ability to search IATI’s entire dataset and carry out complex operations querying IATI’s 200 plus information fields.

Developers will be able to build the API into their applications and execute create, read, update and delete operations on HXS’s IATI clone, giving application users the ability to start, save, edit, share and search information before formally publishing files to IATI as well as test and add information behind experimental non-IATI information fields.

The API is being designed to support and power modern conventional applications as well as emerging new artificial intelligent and blockchain applications.

## Get involved

We can use help to architect HXS, develop and test HXS’s codebase and produce API documentation as well as a help to test and improve the Humanitarian Exchange Server and setup a basic HXS.ngo landing page website giving developers a tool to use to test database query scripts.

To get involved or to learn more about the project, **contact**: hxs(at)beehive.ngo
