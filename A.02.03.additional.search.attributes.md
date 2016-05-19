# A.2.3 Additional search attributes

**Purpose**: Verification whether the additional search attributes are advertised as the results of a Service metadata response to a discover metadata request.

**Prerequisites**

**Test method**

Examine whether the additional search attributes are advertised as a result of a Service metadata response (i.e. a capabilities document) to a Discover Metadata request; i.e. whether the ```OperationsMetadata``` contains the list of search attributes ([AdditionalQueryables](#AdditionalQueryables)).

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 5
* [IR NS](README.md#ref_IR_NS), Annex A

**Test type**: Automated

**Notes**

The XML excerpt of a capabilities document may be found in section 4.4.3. See Implementation Recommendation 1 about internationalisation of the service exceptions.


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="AdditionalQueryables"></a>AdditionalQueryables | /ows:Operation[@name="GetRecords"]/ows:Constraint[@name="AdditionalQueryables"]
