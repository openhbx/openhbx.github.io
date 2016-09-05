---
title: SHOP Special Enrollment Periods
keywords: enroll sep
sidebar: enroll_app_sidebar
toc: true
permalink: ea_shop_seps.html
folder: enroll_app
---
The Enroll Application offers both employee self-attested, and caseworker-managed, Qualifying Life Events and resulting Special Enrollment Periods.  QLE types are fully configurable, with attributes including: title, tool tip, event label, relative order of appearance in QLE list, EDI code, effective on date kinds, SEP time period preceding QLE, SEP time period following QLE and self-attested flag.  For example, following is a QLE definition for birth of child:

* title: "Had a baby",
* tool_tip: "Household adds a member due to marriage, birth, adoption, placement for adoption, or placement in foster care",
* edi_code: "02-BIRTH", 
* effective_on_kinds: ["date_of_event"],
* pre_event_sep_in_days: 0,
* post_event_sep_in_days: 30, 
* is_self_attested: true, 
* ordinal_position: 25,
* event_kind_label: 'Date of birth'

Self-attested QLE’s are available to Employees, and are governed by the configured attributes.  The User Interface guides the employee the SEP creation process step-by-step, presenting appropriate options based on the selected QLE type.  

Following successful creation, the family is eligible to make enrollment changes for the duration of the SEP.

All self-attested and non-self-attested SEPs will be available to caseworkers through the administrator portal to grant SEPs to employees.  This is currently in pre-prod.   Administration SEP types may be configured to provide caseworkers with flexibility to set non-standard start and end dates, and offer multiple effective date options to the employee.   