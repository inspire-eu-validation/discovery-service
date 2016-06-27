# Missing language filter

**Purpose**: Verification whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language.

**Prerequisites**

* [Supported languages](https://github.com/inspire-eu-validation/ats-discovery-service/blob/master/A.02.10.supported.languages.md)

**Test method**

Examine whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language. In other words, if the system under test contains records in more than one natural language, the response shall contain records in several languages, as provided by the INSPIRE Discovery Service Metadata GetCapabilities Document.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Chapter 4.5.2, Implementation Requirement 30

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
