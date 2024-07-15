# Discover Resource Matching Query

**Purpose**: Test that the Discover Metadata response contains at least the INSPIRE metadata elements.

**Prerequisites**

**Test method**

* Send a GetRecords request without any filter.

    * Check that the root of every [Record](#Record) is a MD_Metadata element.

    * Check that the attribute codeListValue of every [MD_ScopeCode](#MD_ScopeCode) is dataset, series or service.

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 12

**Test type**: Automated

**Notes**

Following [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Recommendation 2, the following request parameters will be used:
* `resultType` = `results`
* `outputFormat` = `application/xml`
* `outputSchema` = `http://www.isotc211.org/2005/gmd`
* `ElementSetName` = `full`

The parameter `maxRecords` may be used to limit the number of records to be retrieved.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
Record <a name="Record"></a> | /csw:GetRecordsResponse/csw:SearchResults/*
MD_ScopeCode <a name="MD_ScopeCode"></a> | /csw:GetRecordsResponse/csw:SearchResults/gmd:MD_Metadata/gmd:hierarchyLevel/gmd:MD_ScopeCode
