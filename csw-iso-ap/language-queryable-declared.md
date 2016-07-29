# Language queryable declared

**Purpose**: Verification whether the INSPIRE Discovery Service supports the search criteria (queryable) “language”.

**Prerequisites**

**Test method**

Examine whether the INSPIRE Discovery Service supports the search criteria ([Queryable](#Queryable)) “language” that complies to the metadata element “Metadata language” according to the Commission Regulation 1205/2008.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 20

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="Queryable"></a>Queryable | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="SupportedISOQueryables"]/ows:Value
