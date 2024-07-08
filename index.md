---
layout: default
title: WeatherEye
---

# WeatherEye Overview

WeatherEye is a powerful, integrated suite of free, open-source software created to better support the evolving needs and responsibilities of National Meteorological and Hydrological Services (NMHSs).

<div style="padding:56.25% 0 0 0;position:relative;"><iframe title="vimeo-player" src="https://player.vimeo.com/video/980442634?title=0&byline=0&portrait=0&autoplay=0&dnt=1" width="100%" height="100%" frameborder="0" allowfullscreen></iframe></div>

The suite consists of the following software (each administered through a tab in the WeatherEye admin interface):
1. **DB**: A highly optimised relational database management system (RDBMS)
2. **CDMS**: A system for correctly managing earth system observation data
3. **WIS2**: Software for the discovery and exchange of real-time data using WIS2
4. **API**: Secure, standardised APIs to enable the building of compliant reusable solutions
6. **Portal**: A Content Management System (CMS), fully-integrated to work with the rest of the suite of applications to provide curated access to available data, products and services

In addition, the following solutions are planned:
1. **Tools ⚒️**: A set of tools, unique to WeatherEye, to better manage the integrated set of applications, including tools to correctly update (migrate) database schemas, backup all data and to secure and audit applications
2. **Desktop**: A forecaster desktop solution

WeatherEye builds on existing, high-quality open-source software by integrating these into a single solution with a strong focus on optimising the experience for the user in order to provide accurate and timely weather, climate, and hydrological data management, products and services.

By adopting WeatherEye, NMHSs gain an easier solution for integrating essential software applications and are also guaranteed an easier route to staying up-to-date with WMO advances, including standardisation on first mile data collection, compliance in CDMSs, the standardisation around web APIs and the move to WIS2.

## WeatherEye components

Each of the free, open-source components are described below.

### DB

`Status:` Available, but not yet integrated\
`Powered by:` [CloudBeaver](https://github.com/dbeaver/cloudbeaver) (Apache 2) + PostgreSQL, TimeScaleDB, PostGIS

All of the applications in WeatherEye are underpinned by a free and open-source enterprise-grade database system built on PostgreSQL with extensions for time series (TimescaleDB) and geospatial (PostGIS) data. WeatherEye brings the management of the data associated with each application into a single RDBMS making it easy to secure, backup and maintain.

### CDMS

`Status:` Installable from WeatherEye (SURFACE CDMS install)\
`Powered by:` [SURFACE CDMS](https://github.com/opencdms/surface/) (GPL 3)

WeatherEye uses SURFACE CDMS for it's Climate Data Management System implementation. SURFACE is a complete CDMS solution that can:
- Set up multiple user accounts
- Be configured for use in a specific country
- Manage metadata for station locations, equipment etc.
- Ingest data from multiple sources
- Perform quality control (QC) on data
- Create products

### WIS

`Status:` Available, but not yet integrated\
`Powered by:` [wis2box](https://github.com/wmo-im/wis2box) (Apache 2)

WeatherEye has built-in support to discover, publish and retrieve real-time data from the WIS2 network.

### API

`Status:` In development\
`Powered by:` [OpenCDMS](https://github.com/opencdms/opencdms/) (MIT)

Alongside other applications in the suite, WeatherEye provides a set of interfaces (APIs) that follow the standards being developed by WMO's Expert Team on Information Management. As time progresses, the other WeatherEye components will increasingly uses these standardised interfaces in their implementation.

### Portal

`Status:` Available, but not yet integrated\
`Powered by:` [NMHS-CMS](https://github.com/wmo-raf/nmhs-cms) (MIT)

The portal component uses NMHS-CMS, a shared template for the Wagtail (Python/Django) Content Management System (CMS). WeatherEye will further extend NMHS-CMS to make it simple to add reusable "blocks" that are powered by WeatherEye API.

### Tools ⚒️

`Status:` Not yet available\
`Powered by:` ---

The tools component is unique to WeatherEye and will provide migration, backup, security and other additions that may not be present in the individual solutions.

### Desktop

`Status:` Not yet available\
`Powered by:` [MapStore](https://github.com/geosolutions-it/MapStore2/) (BSD 2)

 A proof-of-concept is in development that uses MapStore as the basis for a web-based forecaster desktop called WeatherEye Desktop. However, this has not yet been made available.


## Conclusion

Roadmap and case study sections will be added to this document in the near future giving more details of the software and timeframes until all components will be made fully available.


https://github.com/weather-eye/weathereye
