# Language search criteria

**Purpose**: Verification whether the INSPIRE Discovery Service supports the search criteria (queryable) “language”.

**Prerequisites**

**Test method**

Examine whether the INSPIRE Discovery Service supports the search criteria ([Queryable](#Queryable)) “language” that complies to the metadata element “Metadata language” according to the Commission Regulation 1205/2008.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 9
* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 20


**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="Queryable"></a>Queryable | ./ows:OperationsMetadata/ows:Operation[name="GetRecords"]/ows:Constraint["name="SupportedISOQueryables"]/ows:Value
