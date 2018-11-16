<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Common data definitions

Common data definitions (also known as the common information model or CIM) create a shared understanding of data.
They are critical where data is to be shared between different systems and or groups of people.

Typically the common data definitions consist of:
* Names and descriptions for concepts described by the data.
* Relationships between these concepts.
* Classifications of the concepts to indicate how they are used.
* Definitions of the valid data values for specific concepts.
* Preferred logical and physical data formats for storing data about these concepts.

The common data definitions are managed in a metadata catalog.  The core definitions that cover the meaning of
data are described in one or more [glossaries](anatomy-of-a-glossary.md).

Governance classifications may be
added to these definitions which in turn link to governance requirements.   This determines how data that is
linked to these common definitions should be governed.

Tools used by the organizaton to, for example, create new data stores, data visualizations, or APIs,
or analytics models are pre-populated with concrete data definitions by
automated tool bridges.
Each tool bridge extracts the relevant definitions from the metadata catalog, generates the concrete definitions
and loads them into the tool.  Where possible, these definitions include tags that link the definitions back to the
common data definitions.

When the new IT capablity is deployed to test and production environments, the tool typically produces a packaged
version of the concrete definitions with their tags that point to the metadata.
The dev-ops pipeline that deploys the artifact reads the tags and ensures that any specific governance requirements for
the specific type of data that is being used are met.

## Further information

* [Common Information Models for an open, analytical and agile world](http://www.ibmpressbooks.com/store/common-information-models-for-an-open-analytical-and-9780133366341)


----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Data Governance project.