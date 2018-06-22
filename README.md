# Onion Architecture Governance Sample

This repository contains a simple sample for implementing architecture governance for an onion architecture with help of
[jqAssistant](http://jqassistant.org) based on stereotypes.

In addition to defining sample concepts and related sample constraints, this repository demonstrates how to include 
jqAssistant rules directly as part of the AsciiDoc-based architecture documentation. 

- Rules are defined directly within the AsciiDoc architecture documentation in `doc/index.adoc` ("single source of 
  truth").
- Rules are validated as part of the maven build process (e.g. using `./mvnw clean install`).
- After running the build, the architecture documentation is available in `generated-docs/index.html`.
- A constraint violation can be force by enabling the commented code in the `AggregateInWrongRing` class, resulting in a
  build failure.
