# INSPIRE metadata elements using ISO 19115/19119 information model

**Purpose**: Verification whether the Discover Metadata response contains at least the INSPIRE metadata elements in each record in the response according to the ISO 19115/19119 information model.

**Prerequisites**

**Test method**

Submit a query without filter and examine whether the Discover Metadata response contains at least the INSPIRE metadata elements in each record, i.e. test whether each [Record](#Record) in the response is a metadata record conforming to the [INSPIRE profile of ISO 19115/19119](http://inspire.ec.europa.eu/id/ats/metadata/1.3/iso-19115-19119).

Following [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Recommendation 2, the following request parameters will be used:
* `resultType` = `results`
* `outputFormat` = `application/xml`
* `outputSchema` = `http://www.isotc211.org/2005/gmd`
* `ElementSetName` = `full`

The parameter `maxRecords` may be used to limit the number of records to be retrieved.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirements 12, 18

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
Record <a name="Record"></a> | /csw:GetRecordsResponse/csw:SearchResults/*
