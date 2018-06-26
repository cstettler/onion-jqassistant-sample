# Onion Architecture Governance Sample

This repository contains a simple sample for implementing architecture 
governance for an onion architecture based on stereotypes with help of
[jQAssistant](http://jqassistant.org) .

In addition to defining sample concepts and related sample constraints, this 
repository demonstrates how to document jQAssistant rules directly in an 
AsciiDoc-based architecture documentation. 

## Rules
Rules are defined in the architecture documentation in `doc/index.adoc` 
("single source of truth") and are validated as part of the maven build
process.

## Documentation
After running the build (e.g. using `./mvnw clean install`), the architecture
documentation is available in `generated-docs/index.html`.

## Triggering Constraint Violations
A constraint violation can be forced by enabling the commented code in one of 
the following classes:

- class `AggregateInWrongRing`
- class `AggregateWithWrongDependencyToApplicationService`

A constraint violation will result in a build failure. 
