# INSPIRE metadata elements

**Purpose**: Verification whether the Discover Metadata response contains at least the INSPIRE metadata elements of each record in the response.

**Prerequisites**

**Test method**

Examine whether the Discover Metadata response contains at least the INSPIRE metadata elements of each resource matching the query.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC),Implementation Requirement 12


**Test type**: Automated

**Notes**

* This test may be tested by ATS-Metadata.
* In order to perform this test using a metadata validator, it will also be necessary to request the response in http://www.isotc211.org/2005/gmd form (outputSchema). This requires the System Under Test to follow [TG DISC](README.md#ref_TG_DISC), Implementation Recommendation 2

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
