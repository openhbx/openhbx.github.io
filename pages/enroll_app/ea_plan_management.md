---
title: Plan Management
keywords: enroll plan management serff puf
sidebar: enroll_app_sidebar
toc: true
permalink: ea_plan_management.html
folder: enroll_app
---
The Enroll Application includes scripts that import plan and dental plans in either SERFF and Public Use Format (PUF) files serialized to XML.  Given the annual frequency and inconsistent quality of these file submissions, these import scripts are routinely run and reviewed by technical staff before publishing to the plan management team.

The data imported from these sources includes plan benefit attributes and rate information. Some benefit values are filtered and transformed to make them suitable for customer presentation on plan selection and shopping comparison Web pages.

Given the annual frequency and inconsistent quality of these file submissions, these import scripts are routinely run and reviewed by technical staff before publishing to the plan management team.

In addition, we have devised a separate process to migrate small groups previously renewing directly with the carriers to DC Health Link. Our system accommodates ingesting employer and employee files from the carriers. The system sets up the employer groups and the employee accounts so that these migrating groups can have a seemless experience transitioning to DC Health Link. We can auto-renew both the group and the group’s employees.

## Plan Review

The Enroll Application includes the capability to analyze, compare and identify differences in plan benefits, deductibles and premiums between plan submissions by carriers. These can include submissions within a single review period, quarterly and annual updates.
More than a month of interactive testing of carriers remotely through secure carrier testing environment. 

## Frozen Plans

The Enroll Application manages and can retain information for active and frozen plans.  At the time of enrollment, the system dynamically determines which plans the employee is eligible to access using (employer-designated) benefit package assignment and coverage effective date.

This separation of concerns between eligibility and enrollment, is a key design feature that enables the Enroll Application to properly manage the complexities of new hires, SEP and renewing employees, and their various combinations.  It also enables proper behavior for time-shifted retroactive coverage, such as COBRA.