# A.3.3 Language search attribute

**Purpose**: Verification whether the language parameter is implemented by using the “language” search criteria (queryable) in a filter statement.

**Prerequisites**

**Test method**

Examine whether the INSPIRE Discovery service implements the “language” parameter by using the Language queryable in a filter statement as defined by an ISO Metadata Application Profile of the OGC Catalogue Service Specification in version 2.0.2. I.e. the Discover Metadata request contains a filter with a [PropertyName](#PropertyName) element "apiso:Language".

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC),Implementation Requirement 10
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 3.1

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="PropertyName"></a>PropertyName | ./csw:GetRecords/csw:Query/csw:ElementSetName/csw:Constraint/ogc:Filter/.../ogc:PropertyName
