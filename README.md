# HXS (Humanitarian Exchange Server)
![HXS Diagram](https://github.com/HXS-API/Server/blob/master/HXS_API.png)
HXS is an open source initiative launched by [Beehive](https://beehive.ngo) volunteers that's bringing humanitarian organizations, tech volunteers and supporters together to setup an **enterprise-grade IATI database**, **server** and **API** for developers to use to prototype and reliably power a whole new generation of sophisticated IATI-data-driven applications.
## Function

**IATI** is a technical framework managed by the [International Aid Transparency Initiative](http://iatistandard.org) that the humanitarian community has been working concertedly to setup and broadly mandate. The framework provides organizations and donors with a channel to openly share detailed information on aid activities, transactions and results and make the information accessible to machine applications.

IATI's [API](https://iatiregistry.org/registry-api) however can only be used to run limited queries and it's not designed to dedicatedly power enterprise-grade applications operating at scale or emerging, highly data-driven, artificial intelligent applications and digital assistants like Alexa and Siri. So we're building an IATI data server and API that are sophisticated and robust enough to suit these needs.

## Project Components

We're organizing the **Humanitarian Exchange Server** into three **components** to work on setting up:

* IATI Data Scraper
* Backend Database
* Server and API

**Scraper**

The IATI Data Scraper will regularly identify the URLs of IATI XML files published by organizations on their own servers, extract file information and combine the information into a time stamped XML file to archive in a file repository. After archiving each file the scraper will process and database each file's information into a single master database.

**Backend Database**

HXS's master backend database will store an up-to-date copy of IATI's entire dataset. Auxiliary databases will store the same data formatted in different manners for testing a variety of storage formats and retrieval techniques as well as store information on IATI file URLs and other information.

**API**

The Humanitarian Exchange Server’s API will give registered developers the ability to search IATI’s entire dataset and carry out complex operations querying IATI’s 200 plus information fields.

Developers will be able to build the API or an auxiliary API into their applications and execute create, read, update and delete operations on HXS’s IATI clone, giving application users the ability to start, save, edit, share and search information before formally publishing files to IATI as well as test and add information behind experimental non-IATI information fields.

The API is being designed to support and power modern conventional applications as well as emerging new artificial intelligent and blockchain applications.

## Get involved

We're looking for more volunteers to help architect the project's different components, develop and test required code and produce API documentation. We're also looking for help to setup an database interface ([HXS.ngo](https://github.com/HXS-API/Website)) giving developers a tool to use to easily test database query scripts and API calls.

To get involved or to learn more about the project, **contact**: hxs(at)beehive.ngo
