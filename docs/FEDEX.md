# FedEx Bar Code Specifications

## Introduction

FedEx has introduced numerous barcodes and standards over the years to improve consistency in numerous areas, such as label readability, fraud prevention, manual override capability, and more. This document will detail some of the common specifications of various labels found in [this documentation](http://www.fedex.com/us/solutions/ppe/FedEx_Ground_Label_Layout_Specification.pdf).

## FedEx Ground "96" Code 128

To begin, the very first code FedEx put to use for their tracking systems in 1986 was named "FedEx Ground '96'", which was a variant of Code 128, first invented in 1981 for use in the military. The FedEx Ground 96 Code has since been in use by FedEx to this very day. The barcode is of a traditional, linear style, with three standard subsets. Below is an image of what the code looks like:

[FedEx Ground 96 Code 128](/images/fedex-ground-96-code-128.png)

The code itself contains three identifier subsets. Subset A encodes uppercase and ASCII characters, Subset B encodes upper and lowercase characters, and Subset C encodes numeric digit pairs from 00 to 99. Pictured is a closer look at the information is encoded:

[FedEx Ground 96 Closer Look](/images/fedex-ground-96-closer-look.png)

## FedEx PDF-417 Two-Dimensional Symbol

Next, a recent innovation by FedEx but originally created by *Symbol Technologies, Inc.* in 1988, the PDF-417 Two-Dimensional Symbol is labeled as a very high-density, low-space consumption, two-dimensional, alphanumeric barcode that consists mainly of a series of linear, vertical barcodes stacked on top of one another. Below is an example of what the barcode looks like:

[PDF 417 2D Symbol](/images/pdf-417-2d-symbol.png)

PDF stands for "Portable Data File", and the nature of the barcode itself grants it the incredible capability of encoding up to a maximum of 2725 separate characters in a single symbol. FedEx, however, only needs to utilize only 350 of these, with the rest being used for compression options, error detection and correction, variable size and aspect ratios, as well as other purposes. Following is a closer look of how it works:

[PDF 417 Closer Look](/images/pdf-417-closer-look.png)

The PDF-417 consists of an array of code words. These are typically small bar and space patterns similar to those on a standard linear barcode. The words are grouped together and stacked to form the symbol. Each symbol consists of at least 3 rows of up to 30 code words each, forming a total of 90 code words per block, which, when stacked together, may contain up to a grand total of 928 code words per symbol. Below is a look at one individual unit:

[PDF 417 Unit](/images/pdf-417-unit.png)

The code words of the PDF-417 symbol are generated using one of the following three data compression modes:

1. Extended Alphanumeric Compaction (EXC)
2. Binary / ASCII Plus
3. Numeric Compaction

Each mode contains its own separate advantages and disadvantages in encoding words. This is usually represented in a balance between security and ambiguity of code words as compared to the amount of information that can actually be encrypted. Generally, with a larger character set, less information can be encrypted, and vice versa. The industry standards for the PDF-417 Two-Dimensional Symbol are listed in the following table. FedEx, as highlighted, requires a security standard of level 5 or higher:

[PDF 417 Security Table](/images/pdf-417-security-table.png)

## SSCC-18 Code 128

Finally, FedEx has additionally provided full system integration for the industry standard SSCC-18 barcode, as originally defined by the Uniform Code Council (UCC). The SSCC-18 is used by FedEx specifically to identify a shipping container for both the shipper and the recipient via an encoded tracking number. The barcode encodes information as follows.

[SSCC-18 Barcode](/images/sscc-18-barcode.png)

Additionally, the barcode incorporates several physical properties, specifically for the purpose of controlling variables like bar height, quiet zone, human readable characters, and overall length. See the image below for more information:

[SSCC-18 Physical Properties](/images/sscc-18-physical-properties.png)