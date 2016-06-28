# Language parameter

**Purpose**: Verification whether the INSPIRE Discovery Service properly supports natural languages.

**Prerequisites**

**Test method**

Examine whether the Get Discovery Service Metadata and Discover Metadata operations support the parameter “language”, which is an INSPIRE extension of the OGC Catalogue Service Specification in version 2.0.2. 

To test the overall language support of a Discovery Service, thee groups of tests need to be performed

1. Testing the language functionality of the Discovery Service on the Get Discovery Service Metadata operation (GetCapabilties)
  * [Request the Discovery Service Metadata in the default language and check in the response whether the service claims to support more than one language](supported-languages.md).
  * Test whether the Get Discovery Service Metadata supports the language parameter
    * [Check whether the GetCapabilities request accepts the parameter "language" containing values based on ISO 639-2/B alpha 3 codes.](iso-639-codes.md)
    * [For a supported but not default language, check for an appropriate response](response-language.md)
    * [Test the response for an unsupported language](unsupported-languages.md)
2. Testing whether the language functionality is advertised correctly in the Discovery Serice Metadata
  * [Check whether GetCapabilities response indicates that the GetRecords operation supports the language parameter as queryable](language-search-criteria.md)
3. Testing the language functionality of the Discovery Serivce on the Discover Metadata operation (GetRecords)
  * [Verify that when no language filter is provided, the GetRecords response returns metadata independent from any language](missing-language-filter.md).
  * [Check whether the language parameter is implemented as a search attribute in a GetRecords request](language-search-attribute.md).
  * [If a language parameter is set, check that the GetRecords response complies with the specified language](language-filter.md).
  * [Verify the language of a GetRecords response to an invalid GetRecords request](invalid-request.md).

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Chapter 4.5, Implementation Requirement 24


**Test type**: Automated

**Notes**
This is a summary test case, providing links to other test cases that satisfy more detailed requirements.

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
