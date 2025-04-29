# WeatherEye Overview

> ⚠️ **Caution:** Not Implemented

WeatherEye is a powerful, integrated suite of free, open-source software created to better support the evolving needs and responsibilities of National Meteorological and Hydrological Services (NMHSs).

## Quick overview

| Name | Capability | Desc | Owner | Existing FOSS used |
|------|------------|------|-------|--------------------|
| [[WeatherEye DCPS]] | Data Collection and Processing System (DCPS) | Extracts data from AWS, Transforms data, Loads data for other services | TBD | Apache Avro, Dagster, Python, MinIO |
| [[WeatherEye Broker]] | WIS2 Node | A broker to discover, publish and retrieve real-time data to/from the WIS2 network | [WMO](https://github.com/World-Meteorological-Organization) | wis2box, Python, MioIO, docker, mosquitto (mqtt) |
| [[WeatherEye CMS]] | Content Management System (CMS) | Customisation to Wagtail for NMHSs| [wmo-raf](https://github.com/wmo-raf) | Python, Django, Wagtail, PostgreSQL |
| [[WeatherEye CDMS]] | Climate Data Management System (CDMS) | System for correctly managing and archiving earth system observation data | Currently [openwis](https://github.com/openwis) | Django, Python, PostgreSQL, TimescaleDB, PostGIS |
| [[WeatherEye API]] | Application Programming Interface (API) | WMO-compliant (in collab. with [ET-IM](https://github.com/wmo-im/et-im) | Currently [openwis](https://github.com/openwis) | opencdms, pygeoapi, python |

## Complete overview

The suite consists of the following main modules (each administered through a tab in the WeatherEye admin interface):

**NOTES**\
&nbsp;&nbsp;  📦 Indicates use of an existing software (with necessary configuration)\
&nbsp;&nbsp;  🆕 Indicates development of new software required\
&nbsp;&nbsp;  ✨ Indicates required solution is only partially solved and is still being considered 

**WeatherEye Admin:** Core admin services (server management and security)
  - [[WeatherEye Auth]] 📦 
  - [[WeatherEye Backup]] ✨
  - [[WeatherEye Monitor]] 📦
  - [[WeatherEye Proxy]] 📦  
  - [[WeatherEye Upgrade]] ✨

**WeatherEye Capsules:** Reusable framework-agnostic processes and components
- [[WeatherEye Capsules]] ✨ consist of
  - OGC API - Processes
  - W3C Web Components
  - Gherkin tests for processes and components
  - Documentation

**WeatherEye Config:**
- [[WeatherEye OS]] (WOS) 📦 Install on a dedicated server that has no operating system installed (requires physical access to machine and USB memory stick)
- [[WeatherEye Controller]] (WXC) 🆕 Install on an existing Linux server, including in the cloud (requires SSH access to remote machine)
- [[WeatherEye Setup]] (WXS) 🆕 Install a version of the controller on your local MacOS, Windows or Linux desktop machine in order to provision new server infrastructure and then install and configure WeatherEye on those servers

**WeatherEye Datastore**: Data storage and management
  - [[WeatherEye CDMS]] 📦 A system for correctly managing earth system observation data
  - [[WeatherEye RDBMS]] 📦 A highly optimised relational database management system with admin tools (RDBMS)
  - [[WeatherEye Filestore]] 📦 A manage filestore using S3 buckets (MioIO can allow FTP/SFTP access)

**WeatherEye Forecast**: Forecaster applications
  - [[WeatherEye Forecaster Desktop]] 🆕 A forecaster desktop solution
  - [[WeatherEye Information Management]] 🆕 An admin tool for forecasters to manage information displayed on the public website 

**WeatherEye Hub**: Central Data Hub
  - [[WeatherEye API]] 🆕 Secure, standardised APIs to enable the building of compliant reusable solutions
  - [[WeatherEye DCPS]] 🆕 A Data Collection and Process System (DCPS) responsible for Extracting data from Automatic Weather Stations (AWS), Transforming data (aggregation and encoding) and Loading the data into other systems including the CDMS and sharing on WIS2
  - [[WeatherEye Broker]] 📦 Software for the discovery and exchange of real-time data on WIS2 using mqtt

**WeatherEye Portal**: Customer facing applications
  - [[WeatherEye App]] ✨ An installable mobile app providing essential information and WeatherEye Warn alerts
  - [[WeatherEye CMS]] 📦 A Content Management System (CMS), fully-integrated to work with the rest of the suite of applications to provide curated access to available data, products and services - ClimWeb
  - [[WeatherEye Helpdesk]] 📦 A ticket tracking system to run a support desk (for internal and external requests)
  - [[WeatherEye Warn]] ✨ A system for issuing early warnings

WeatherEye builds on existing, high-quality open-source software by integrating these into a single solution with a strong focus on optimising the experience for the user in order to provide accurate and timely weather, climate, and hydrological data management, products and services.

By adopting WeatherEye, NMHSs gain an easier solution for integrating essential software applications and are also guaranteed an easier route to staying up-to-date with WMO advances, including standardisation on first mile data collection, compliance in CDMSs, the standardisation around web APIs and the move to WIS2.

<br><br>

<details>
  <summary>Developer notes (click to expand)</summary>
  
The WeatherEye docs are build from this wiki. WeatherEye follows Documentation Driven Development (DDD). The docs are written first and then the software is written to fulfil the capabilities described in the docs. Below is an example of an unimplemented section.

> ## Example section
>
> ⚠️ **Caution:** Not Implemented
>
> This is an example describing a feature that has not yet been implemented

</details>