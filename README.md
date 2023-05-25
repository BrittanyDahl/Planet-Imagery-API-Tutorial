Planet-Imagery-API-Tutorial
---
1. Introduction
---
This tutorial is an introduction to Planet's APIs, including the Data API. It provides code samples on how to write simple Python code to access Planet Satellite Imagery data.

The focus of this tutorial will be the search portion of the Planet Data API. We will find and download imagery data using complex searches and save them for later use, as well as learn how to get stats on search results. After completing this tutorial, you should feel comfortable interacting with the Data API, and have a good foundation for leveraging the Planet Data API for your own applications.

Please note that you may benefit from prior experience with Python and using Planet imagery, but this is not required to complete the activity. 

This script was presented to QLD Government Planet users in the QLD Government Planet Imagery Automation with Scripting APIs Virtual Training on the 22nd of May 2023.
---
2. Resources
---
---
2.1. Set-up instructions
---
This training script can run directly in your browser (no setup required!) using the [Google Colaboratory platform](https://colab.research.google.com/). Colaboratory is supported on most major browsers, and is most thoroughly tested on desktop versions of Chrome and Firefox. For more information about Colab please visit [FAQs](https://research.google.com/colaboratory/faq.html). 

Please note that running through Colab will require sharing of your API key and licensed data in a personal Google account. We recommend following Planet’s security advice for using API Keys [here](https://developers.planet.com/docs/basemaps/tile-services/#api-key-security-risk).
If you'd prefer to download and run the Notebook (.ipynb) in another program, you can utilise Jupyter Notebooks (installed with Anaconda or ArcGIS Pro) or Python. Please note that this process is likely complicated due to internal proxy and firewall settings, and requires local installation of required packages. If you need assistance with installation of these programs please contact your agency's IT support area. For all other querys, please contact State Imagery: imagery@spatial-qld-support.atlassian.net.
---
2.2. Resources
---
We recommed familiarity with the following resources:

*   [Planet API Documentation](https://developers.planet.com/docs/apis/)
*   [Planet GitHub Jupyter Notebooks](https://github.com/planetlabs/notebooks/tree/master/jupyter-notebooks)
*   [More Data API Notebook Tutorials](https://github.com/planetlabs/notebooks/tree/master/jupyter-notebooks/data-api-tutorials)
*   [API Status Page](https://status.planet.com/)
*   [Planet Account Page for your API Key](https://www.planet.com/account)
*   [Date-Time Converter](https://it-tools.tech/date-converter)
*   [Geojsonio](https://geojson.io)

Please note that Planet have several APIs, including:
*   Data API - allows you to search Planet's complete catalog of data
*   Orders API - raster tools for creating analysis-ready data with Planet's archive
*   Subscriptions API - allows you to subscribe to continuous cloud delivery of imagery and metadata collections
*   Basemaps API - give you access to Planet's mosaiced basemap services
*   Tile Services API - XYZ and WMTS tile map services for use in your favourite GIS or mapping client
*   Reports API - API which systematically reports download usage for internal processing and analysis
*   Tasking API - API for creating and managing your SkySat point collection orders
*   Analytics API - gives you access to derived analytic products (Planet Analytic Feeds)
---
2.3 Prerequisites
---
*   Planet QLD Government Account
  *    If you do not have an account, please request an account using the following [link](https://spatial-qld-support.atlassian.net/servicedesk/customer/portals?q=QSat+access+request) or contact imagery@spatial-qld-support.atlassian.net. 
*   Planet API Key (available in the [Account page settings](https://www.planet.com/account) for Planet QLD Government Account holders)
*   Google Colab, Jupyter Notebooks or Python environment
