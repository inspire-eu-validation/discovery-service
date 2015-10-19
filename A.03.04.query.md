# A.3.4 Query

**Purpose**: Verification whether the query parameter is implemented by the filter statement of the Discover Metadata request itself.

**Prerequisites**

**Test method**

Examine whether the query parameter is implemented by the filter statement of the Discover Metadata request itself. Examine whether the query may support all the following search attributes: Keyword, Topic category, Spatial data service type, Lineage, Spatial resolution, Specification, Degree, Geographic bounding box, Conditions applying to access and use, Limitations on public access, Responsible party, Responsible party role, Resource Title, Resource Abstract, Resource Type, Unique resource identifier, Temporal Reference, Degree, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), LimitationsOnPublicAccess (composed of AccessConstraints, OtherConstraints, Classification), Conditions applying to access and use, Lineage, ResponsiblePartyRole, intersects.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 11
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 3.1

**Test type**: Automated

**Notes**

The list in the Technical Guidance does not correspond to the list in Commission Regulation No 976/2009. The legally binding document also defines intersects as a spatial operator, however such information is not advertised in the Technical Guidance document. See Implementation Recommendation 2 about a common structure of the request parameters and appropriate responses.


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
