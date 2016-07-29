# Language filter

**Purpose**: Verification whether the language parameter is implemented by using the “language” search criteria (queryable) in a filter statement and whether the response to a Discover Metadata request comply with a language defined in the request.

**Prerequisites**

**Test method**

* For each [SupportedLanguage codes](#supported-languages) as ```lang-code```:
  * Create a GetRecords request with a query that includes only the language queryable (a filter with a [PropertyName](#PropertyName) element "apiso:Language") with a predicate that the value must be equal to `lang-code`. Use the following request parameters:
    * `resultType` = `results`
    * `outputFormat` = `application/xml`
    * `outputSchema` = `http://www.isotc211.org/2005/gmd`
    * `ElementSetName` = `full`
    * The parameter `maxRecords` may be used to limit the number of records to be retrieved, but should not be smaller than 5.
  * Execute the request. 
  * Check that the response is a `csw:GetRecordsResponse` document.
  * Check that each all [language](#language) nodes have the value `lang-code`. Note that there may be no such nodes in the response.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirements 10, 31

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="PropertyName"></a>PropertyName | /csw:GetRecords/csw:Query/csw:ElementSetName/csw:Constraint/ogc:Filter//ogc:PropertyName
language <a name="language"></a> | /csw:GetRecordsResponse/csw:SearchResults/gmd:MD_Metadata/gmd:language/gco:CharacterString
