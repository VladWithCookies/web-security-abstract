# XML Injection

## Description
XML Injection is ability to manipulate an application's XML parser into loading user-supplied external entities.

## Prevention
Configure applications XML parsers to disable the parsing of XML eXternal Entities (XXE) and Document Type Definitions (DTD) when parsing XML documents 
or disable the parsing of external general entities and external parameter entities when parsing untrusted XML files.

