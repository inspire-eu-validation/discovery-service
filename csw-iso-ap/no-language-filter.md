# No language filter

**Purpose**: Verification whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language.

**Prerequisites**

* [Supported languages](supported-languages.md)

**Test method**

Examine whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language. In other words, if the system under test contains records in more than one natural language, the response shall contain records in several languages, as provided by the INSPIRE Discovery Service Metadata GetCapabilities Document.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.5.2, Implementation Requirement 30

**Test type**: Manual

**Notes**

This test case could be automated, if the list of languages used in metadata records is provided as a parameter.  

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
