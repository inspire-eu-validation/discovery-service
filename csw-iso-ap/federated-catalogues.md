# Federated catalogues advertisement

**Purpose**: Verification whether all federated catalogues have been advertised as a result of a Service metadata response to a Discover Metadata request.

**Prerequisites**

**Test method**

Examine whether all federated catalogues have been advertised as a result of a Service metadata response (i.e. a Capabilities document) to a Discover Metadata request; i.e. whether the ```OperationsMetadata``` contains ```Constraints``` element with name=”[FederatedCatalogues](FederatedCatalogues)” attribute and included links to all federated catalogues. A federated catalogue must be advertised as the URL of its HTTP/KVP/GET Capabilities document.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapters 4.2, 4.3.4.3, Implementation Requirements 3, 16

**Test type**: Manual

**Notes**

The XML excerpt of a capabilities document may be found in section 4.3.4.3.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="FederatedCatalogues"></a>FederatedCatalogues | /ows:OperationsMetadata/ows:Constraint[@name='FederatedCatalogues']
