# Migration-2.0-to-3.0
Migration from DigitalState platform 2.0 to 3.0: Instructions, helper scripts, and documentation about migrating from DigitalState platform 2.0 to 3.0


# Overview

The change from 2.0 to 3.0 is a internal structral change without changing core business functions.  Each business entitiy remains the same in version 3.0, but the entities have been decoupled from a central monolith into standalone microserivces and a javascript adminstrative and portal UI.  Each microservice manages its own database.


**This repository contains the following:**

### Per-microservice migration instructions and scripts

...


### BPMN files for bulk transfers

A series of BPMN files that are configurable to migrate content from a 2.0 instance to a 3.0 instance.

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

Special care should be used when migrating users (usernames/passwords, etc) from 2.0 to 3.0 instance.

Considerations:

...


# Breaking changes

Listing of breaking changes between 2.0 and 3.0.

Migrations are provided wherever possible, but some changes require manual intervention if your 2.0 instance has been modified beyond core DigitalState fields.

...


# Camunda Migration

1. BPMN Updates
1. Database updates
1. Supported Camunda Server versions
1. API Changes


# User Interface Migrations

...


# Translated Content Migration Considerations

...


# Forms Considerations

...