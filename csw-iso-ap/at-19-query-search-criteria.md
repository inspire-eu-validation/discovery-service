# Query Search Criteria

**Purpose**: Test that the Discover Metadata service supports queryables.

**Prerequisites**

**Test method**

* Check manually if the service response is correct while using the following queryables in GetRecords requests:

    * Keyword, Topic category, Spatial data service type, Lineage, Spatial resolution, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), Degree, Geographic bounding box, Conditions applying to access and use, Limitations on public access (composed of AccessConstraints, OtherConstraints, Classification), Responsible party, Responsible party role, Resource Title, Resource Abstract, Resource Type, Unique resource identifier, Temporal Reference

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 19

**Test type**: Manual

**Notes**

The queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 4.

Limitations: It is not possible to test this requirement automatically. Although it is possible to send GetRecords requests to the service using the queryables described above, it is not possible to know which values shall be used in the query nor to know if the response is correct.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
