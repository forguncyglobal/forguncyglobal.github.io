---
layout: default
title: Barcode
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Barcode/
nav_order: 22
---

# {{ page.title }}

Create a barcode with this cell type.

There are following barcodes that can be set in the Forguncy:

- QRCode
- NW7 (Codabar, Codeabar, Code2of7)
- CODE39
- GS1-128 (EAN128, UCC/EAN-128)
- CODE128
- JAN13 (EAN13)

![barcode_celltype](/assets/images/product-images/barcode_celltype.png)
{:.dropshadow}

Steps to create a Image Uploader cell type:

- Select cell and go to the **Cell Type** drop-down list. 
- Select **User Selector** cell type. 
- The selected cell becomes a Barcode type.
- Go to the **Cell Type** tab at the bottom of the right pane to configure the barcode .
You can do the following settings from here:

![barcode_celltype_settings](/assets/images/product-images/barcode_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Barcode Type|Select the barcode type from the dropdown list.|
|Check Digit|Check to add a check digit.|

The setting values ​​that only specific barcode types support are as follows:

||QR Code|NW7|
|:--|:--|:--|
|Version|Set the version of QRCode (size of data amount that can be expressed by QRCode).||
|Concatenation|Enables concatenation function.||
|Concatenated number|This can be set only when **Concatenation** is enabled. Allows to set the concatenated number.|
|Check Digit Algorithm||Set the check digit calculation method (algorithm).|

For GS1-128 (EAN128) and CODE-128 barcode types, the following keywords can be used to output function characters FNC1 to FNC4.

|Function character|Keyword|
|:--|:--|
|FNC1|%FNC1%|
|FNC2|%FNC2%|
|FNC3|%FNC3%|
|FNC4|%FNC4%|

![barcode_celltype_codetype](/assets/images/product-images/barcode_celltype_codetype.png)
{:.dropshadow}

- Data concatenation is performed as necessary.