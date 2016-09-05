---
title: Benefit Enrollment
keywords: edi benefit enrollment maintenance asc x12 5010
sidebar: hix_app_sidebar
toc: false
permalink: hix_benefit_enrollment.html
folder: hix_app
---

## EDI Enrollment and Maintenance Transactions

The EDI Application produces and consumes EDI messages complaint with the ASC X12 5010 protocol.  The system generates 834 Benefit Enrollment and Maintenance files for SHOP enrollments.  DC Health Link has developed and documented supplemental guidance for specific transactions types, and expects to do the same to meet the needs of the Health Connector and its trading partners.

## Audit Files

The EDI application can generate 834 audit files on a periodic or ad hoc (on demand) basis.

The EDI Application can generate 834 audit files comparing trading partner enrollment systems. DC Health Link has specified detailed guidance for generating 834 audit files, and expects to use this as the basis for Health Connector requirements. 

## TA1/999

The EDI Application generates and receives ASC X12 TA1/999 files to signal errors with an overall transmission, or individual transactions.  Additionally, the DC Health Link has developed a  functional error protocol that builds upon the syntactical checks of the TA1/999 and low level SNIP checks.