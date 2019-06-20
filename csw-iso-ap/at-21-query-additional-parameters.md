# Query Additional Parameters

**Purpose**: Test that the Discover Metadata service supports additional queryables.

**Prerequisites**

**Test method**

* Check manually if the service response is correct while using the following queryables in GetRecords requests:

    * Degree, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), Limitations on public access (composed of AccessConstraints, OtherConstraints, Classification), ConditionApplyingToAccessAndUse, Lineage, ResponsiblePartyRole

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 21

**Test type**: Manual

**Notes**

The queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 5, 6 and 7.

Limitations: It is not possible to test this requirement automatically. Although it is possible to send GetRecords requests to the service using the queryables described above, it is not possible to know which values shall be used in the query nor to know if the response is correct.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
