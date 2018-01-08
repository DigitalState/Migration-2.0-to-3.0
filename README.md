# Migration-2.x-to-3.x

Migration from DigitalState platform 2.x to 3.x: Instructions, helper scripts, and documentation about migrating from DigitalState platform 2.x to 3.x


# Overview

The change from 2.x to 3.x is a internal structural change without changing core business functions.  Each business entity remains the same in version 3.0, but the entities have been decoupled from a central monolith into standalone microserivces and a javascript administrative and portal UI.  Each microservice manages its own database.


**This repository contains the following:**

### Per-microservice migration instructions and scripts

...


### BPMN files for bulk transfers

A series of BPMN files that are configurable to migrate content from a 2.x instance to a 3.x instance.

BPMN Files:

1. [Cases](#)
1. [Communications](#)
1. [Interactions](#)
1. [Users](#)
1. [Personas](#)
1. [Tasks](#)
1. [Records](#)
1. [Assets](#)
1. [Topics](#)
1. [Services](#)



### User Account Migration Instructions

Special care should be used when migrating users (usernames/passwords, etc) from 2.x to 3.x instance.

Considerations:

...


# Breaking changes

Listing of breaking changes between 2.x and 3.x.

Migrations are provided wherever possible, but some changes require manual intervention if your 2.0 instance has been modified beyond core DigitalState fields.

...


# Camunda Migration

1. BPMN Updates
1. Database updates
1. Supported Camunda Server versions
1. API Changes

## Unit Testing

All processes should be unit tested before performing a migration.  Migration cannot be guaranteed without unit tests.

Use DigitalState's [configurations and examples](https://github.com/DigitalState/Camunda-Spock-Testing) of Spock Framework to build Cucumber Style Unit Tests.

Scripts such as Javascript and Groovy that get executed during the process can also be unit tested with the same framework.  See the [End-to-End example](https://github.com/DigitalState/Camunda-Spock-Testing/tree/master/End-to-End) for Nashorn Javascript unit testing.

## Camunda Version

The Jsoup library is recommended for doing data migrations from 2.x to 3.x.  The camunda-variations repository provides a [working example](https://github.com/DigitalState/camunda-variations/tree/master/web-scrape), documentation, and code samples on how to install Jsoup and leverage the HTTP request power of Jsoup.


# User Interface Migrations

...


# Translated Content Migration Considerations

Translation files are converted into JSON format and migrated into the CMS microservice.  See the `data` entity type in the CMS microservice for JSON format support.


# Forms Considerations

1. Custom forms can be manually migrated.
1. Formio forms can be migrated by transferring the same mongo database into the 3.x deployment.
