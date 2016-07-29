# INSPIRE queryables

**Purpose**: Verification whether the INSPIRE Discovery Service supports the search criteria (queryables) as indicated in Table 4.

**Prerequisites**

**Test method**

Examine whether the INSPIRE Discovery Service supports all the following search criteria (queryables) using `csw:GetRecords` requests: Keyword, Topic category, Spatial data service type, Lineage, Spatial resolution, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), Degree, Geographic bounding box, Conditions applying to access and use, Limitations on public access (composed of AccessConstraints, OtherConstraints, Classification), Responsible party, Responsible party role, Resource Title, Resource Abstract, Resource Type, Unique resource identifier, Temporal Reference.

This will require determining query predicates for each queryable. In general, this will require submitting queries to determine values that can be used in predicates.

The response to each query must be a `csw:GetRecordsResponse` document.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.4.2, Implementation Requirement 19, 21

**Test type**: Automated

**Notes**

Tables 5, 6 and 7 have additional information needed to execute tests (in addition to the CSW and CSW ISO AP standards).

The metadata records in the responses do not need to be validated, this is already covered by test case [INSPIRE metadata elements using ISO 19115/19119 information model](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-metadata-elements).

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
