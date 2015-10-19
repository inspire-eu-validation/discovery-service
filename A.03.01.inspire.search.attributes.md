# A.3.1 INSPIRE search attributes

**Purpose**: Verification whether the additional search attributes listed in Section 4.4 are supported by a discovery service.

**Prerequisites**

**Test method**

 Examine whether a discovery service supports the additional search attributes listed in Section 4.4, i.e. Keyword, Topic category, Spatial data service type, Lineage, Spatial resolution, Specification, Degree, Geographic bounding box, Conditions applying to access and use, Limitations on public access, Responsible party, Responsible party role, Resource Title, Resource Abstract, Resource Type, Unique resource identifier, Temporal Reference, Degree, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), LimitationsOnPublicAccess (composed of AccessConstraints, OtherConstraints, Classification), Conditions applying to access and use, Lineage, ResponsiblePartyRole, intersects.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC),Implementation Requirement 4 and section 4.4
* [IR NS](README.md#ref_IR_NS) Annex II – Part A

**Test type**: Automated or Manual?

**Notes**

The list in the Technical Guidance does not correspond to the list in Commission Regulation No 976/2009. The legally binding document also defines intersects as a spatial operator, however such information is not advertised in the Technical Guidance document.

The test is an abstraction of the tests A.3.7 INSPIRE search criteria test A.3.8 Language search criteria test, A.3.9 Additional search criteria test.


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
