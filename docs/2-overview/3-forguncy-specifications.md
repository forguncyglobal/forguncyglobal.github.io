---
layout: default
title: Forguncy Specifications
parent: Overview
permalink: /overview/forguncy-specifications/
nav_order: 3
---

# {{ page.title }}

This page describes the specifications of Forguncy.

## Table (Forguncy Internal Database)

|Controls|Maximum Size Limit|
|:--|:--|
|Table name|128 characters|
|Field name|128 characters|
|Number of fields in one table|2,000|

|Data Type|Range|
|:--|:--|
|Text|1,000,000,000 bytes|
|Integer|-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 15 significant digits|
|Decimal|-1.7E+308 to -5.0E-324, 0, and 5.0E-324 to 1.7E+308 15 significant digits including integer and fractional digits|
|Date Time|0100/1/1 00:00:00 (serial number: -657434) to 9999/12/31 23:59:59 (serial number: 2958465.99999)|
|Yes/No|A value that is either 1 (True) or 0 (False) or null|
|User account|The user name of a user registered as a user account for form authentication of Forguncy conforming to the user name that can be registered with Forguncy is 50 characters or less.|
|Image maximum file name length| + 37 characters|
|Attachment	maximum file name length| + 37 characters|

- All data types support null value.
- The maximum size that can be used as the database data area is 2 TB for one application (project).
- The following characters cannot be used in table names or field names.

    - \ / : * ? " < > -~ @ # $ ^ % & + = ` ' . , ; ! ) |
    - Full-width Arabic numerals
    - White space
    - Single-byte numbers cannot be used as the first character.
- If the processing of one query to the database inside Forguncy exceeds 30 seconds, the processing will time out and fail.
- Empty characters are not supported. It is treated as a non-input state (Null value).
- If the rounding value of the ROUND function is 5, the result may not be what you intended. Cases where ROUND(2.125,2)→2.12 and ROUND(32.995,2)→32.99 have been confirmed. If you need to calculate strictly, please consider using an external database.

## Page

|Function|Maximum value|
|:--|:--|
|Worksheet size|999 rows, 999 columns|
|Column width|Depends on available memory. *Maximum value for Excel is 255 characters. This corresponds to 1,790 pixels for Forguncy.|
|Line height|Depends on available memory. *Maximum value for Excel is 409 points. This corresponds to 546 pixels for Forguncy.|
|Total number of characters the cell can contain|Depends on available memory. *The maximum value for Excel is 32,767 characters.|
|The number of significant digits that the cell can display and calculate|15 digits|

- The following characters cannot be used in page names (the same applies to names of server-side commands and scheduled tasks).
    - \ / : * ? " < > # % & + = ' , ; ! |
    - Full-width Arabic numerals
    - Single-byte numbers cannot be used as the first character.

## Team Collaboration

Threshold for the Git hosting services is:

|Threshold type|Threshold|
|:--|:--|
|Git repository size|1GB|
|File size|100MB|

