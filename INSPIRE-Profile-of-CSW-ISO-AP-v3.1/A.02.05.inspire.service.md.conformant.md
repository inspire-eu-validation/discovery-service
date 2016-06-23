# A.2.5 INSPIRE service metadata conformant

**Purpose**: Verification whether the Get Discovery Service Metadata response provides a document that is in conformance with the requirements of INSPIRE service metadata.

**Prerequisites**

* [Discovery Service Metadata Parameters](https://github.com/inspire-eu-validation/ats-discovery-service/blob/master/A.02.04.discovery.service.metadata.parameters.md) returns scenario 2

**Test method**

Examine whether the Get Discovery Service Metadata response provides a document that is in conformance with the requirements of INSPIRE service metadata as defined in the Commission Regulation No 1205/2008.

Test whether all 13 mandatory elements are non-empty strings, furthermore if the type of the element is a URI, ping the URL to check that it is valid. If the element is a date, check that are formatted correctly as YYYY-MM-DD.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 8
* [IR NS](README.md#ref_IR_NS), Article 2
* [IR MD](README.md#ref_IR_MD)

**Test type**: Automated

**Notes**
XPath expressions for each of the necessary elements are given in Table 3 of [TG DISC](README.md#ref_TG_DISC)

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
