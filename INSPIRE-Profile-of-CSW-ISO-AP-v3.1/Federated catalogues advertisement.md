# Federated catalogues advertisement

**Purpose**: Verification whether all federated catalogues have been advertised as a result of a Service metadata response to a Discover Metadata request.

**Prerequisites**

**Test method**

 Examine whether all federated catalogues have been advertised as a result of a Service metadata response (i.e. a capabilities document) to a Discover Metadata request; i.e. whether the ```OperationsMetadata``` contains ```Constraints``` element with name=”[FederatedCatalogues](FederatedCatalogues)” attribute and included links to all federated catalogues.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Chapter 4.2, Implementation Requirement 3

**Test type**: Manual

**Notes**

The XML excerpt of a capabilities document may be found in section 4.3.4.3

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="FederatedCatalogues"></a>FederatedCatalogues | /ows:OperationsMetadata/ows:Constraint[@name='FederatedCatalogues']
