---
title: Release Management
keywords: software development lifecycle sdlc
sidebar: dpb_sidebar
toc: false
permalink: dpb_release_management.html
folder: playbook
---
Coordinating contributions from dozens of developers, the DCHBX team oversees a structured, automated code management process, subject to rigorous quality assurance.  Following is an overview of the development and release management process.

All software development—ranging from complex new subsystems to simple text changes—is anchored to a feature or issue recorded in the issue tracking system. Stakeholders, business analysts, and developers collaborate to capture specifications as in structured use case and user story form, including executable Cucumber/Gherkin files.

Next, developers create a new github branch to manage their project work.  Applying Behavior Driven Development, the developers first build and extend automated tests and specifications using Rspec and Cucumber, to enumerate business rules and verify expected User Interface behavior.  Software code follows, using red/green/refactor process.

Completed code is merged into the github repository in the initial integration test environment, and regression tests are automatically run by the continuous integration service.  When regression tests fail, the developer is notified via Slack of the failure along with the reason(s) and links to the logged errors.  Failed tests “break the build”, and the developers must immediately repair or revert the code changes.

When regression tests succeed, the code is automatically promoted and deployed to the functional test environment.  At this stage, testers conduct tests to verify the proper integration with the system and confirm that capabilities match specified requirements.  As the new software progresses through the integration and test process, the code is promoted up through progressively advanced environments, including test, UAT, pre-production and production.  

Stakeholders perform the final feature review for complete and correct operation.  Once the stakeholder accepts the feature, the software is tagged and committed to the master branch in the shared github repository and automatically deployed to production.

The standard Enroll Application configuration is a multiple node cluster, enabling new software deployment to occur on one node at a time, without taking the system offline.  The result is Zero Downtime deployment. 
