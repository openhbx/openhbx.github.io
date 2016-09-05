---
title: Employer Group Files
keywords: enroll document management
sidebar: enroll_app_sidebar
toc: false
permalink: ea_employer_group_files.html
folder: enroll_app
---
The Enroll Application SHOP platform includes an automated process to generate event-driven employer/group XML files for carrier partners. Among other events, XMLs are generated when groups are effectuated, renewed, or terminated. The platform also supports manual generation of group XML files. 

Prior to transmission, employer events are sorted based on benefit package definition, so that carriers receive information only for employers that they service. 

The group XML files were initially generated and dropped on a monthly basis, reflecting additions and updates during the prior month.  Under new development, these are produced on a daily basis, as needed, organized into digests of that day’s activity.  

These group files are part of a larger controlled vocabulary for health benefit exchanges, called the ACApi Canonical Vocabulary (CV).  The CV was developed by DCHBX and is published under an open source license for use by others.  See: https://github.com/dchbx/cv

Employer group events transmitted to carriers include:

* benefit_coverage_initial_application_eligible
* address_changed
* contact_changed
* fein_corrected
* name_changed
* broker_added
* broker_terminated
* general_agent_added
* general_agent_terminated
* benefit_coverage_period_terminated_voluntary
* benefit_coverage_period_terminated_nonpayment
* benefit_coverage_period_terminated_relocated
* benefit_coverage_renewal_application_eligible
* benefit_coverage_renewal_carrier_dropped
* benefit_coverage_renewal_terminated_voluntary
* benefit_coverage_renewal_terminated_ineligible
* benefit_coverage_period_reinstated

