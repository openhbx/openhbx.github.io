---
title: Development Methodology
keywords: software development lifecycle sdlc
sidebar: dpb_sidebar
toc: false
permalink: dpb_development_methodology.html
folder: playbook
---
## Software Development Methodology

The DCHBX Application Development Team (AppDev) is comprised of highly skilled engineers versed in modern system architecture design and developers who possess the expertise necessary to author reliable and highly performant software designed specifically for state-based health insurance marketplaces.

Under DCHBX&#39;s Agile development method, system requirements are rapidly prototyped to describe initial ideas and the requirements are iterated with our stakeholders participating as co-developers.

Agile development is a full lifecycle, collaborative, iterative method of determining requirements and developing engineering and IT project solutions using cross-functional teams of subject matter experts and developers. Agile software development cycles are iterative, with time periods between gathering Use Case requirements and releasing software measured in periods of weeks.

Our Agile methodology calls for breaking large or complex projects down into short-duration iterations that may be completed in 90 days or less as prioritized by the HIX Community Member stakeholders. Each iteration cycle sets a fixed timeframe, defines labor resources, and culminates in the delivery of useful system functionality as articulated in the form of User Stories. User Stories are short descriptions of system capabilities and expected behaviors from the perspective of stakeholders who will use the system.

During the requirements gathering process, the DCHBX team facilitates Joint Application Development (JAD) sessions with HIX Community Member stakeholders to elaborate these requirements and state them in terms of business goals, or Use Cases. Use Cases describe functional requirements in the form of precise scenarios at the user&#39;s goal level.

The DCHBX development workbench applies a number of strategies and tools to provide HIX Community Member stakeholders with high visibility during system development activities and promote collaboration between team members.  These workbench tools include:

* **Knowledge base** : a collaborative environment for capturing system requirements, design artifacts and documentation
* **Issue tracking** : create, update, resolve and track reported system bugs, features and issues
* **Software version control repository** : a distributed database that enables developers to commit, rollback and tag software versions
* **Continuous integration** : tools that perform comprehensive regression tests on new and updated software, and automatically deploys passing software to test environment servers
* **Test environments** : provides business stakeholders early access to software in under development

Our experience shows that casting system capabilities in terms of business drivers:

* Produces software that is better aligned with organization processes
* Helps the project team identify, prioritize and maintain focus on success elements
* Enables leaders and managers to understand how the result will benefit the organization&#39;s mission
* Provides a basis for justifying and allocating appropriate resources and calculating return on investment

Under the DCHBX Agile development methodology, HIX Community Member partners are assured delivery of production systems that fulfill business needs on-schedule and within budget. To support this collaborative approach, DCHBX will provision and maintain a coordinated system development environment for the duration of each project.

Our process typically consists of the following steps:

1. System Standup
2. Prepare Software Development Environment
3. Define Requirements through Use Cases
4. Elaborate Use Cases, Design System and Data Model
5. Develop and Test Software
6. Migrate Data into the New System

## Step 1: System Standup
The system setup phase includes tasks that size, specify, and implement cloud infrastructure for development and production system environments.  The DCHBX DevOps team prepares AWS Cloud specifications which are sized and configured to meet and exceed projected HIX Community Member traffic volume and loads in development and production environments. Cloud infrastructure design and specifications are reviewed with representatives of each HIX Community Member prior to system stand-up.

Additional system standup preparations include the DCHBX Business Lead meeting with the HIX Community Member business team to obtain digital assets, including logos and color schemes to match the look and feel of their existing online systems.  Website branding, content and styling are applied to produce and deploy an &#39;Enroll Application&#39; instance that is customized to meet the HIX Community Member partner&#39;s needs.

In order to meet and exceed federal security requirements, cloud components are hosted on a FedRAMP-compliant, Federal Information Security Management Act (FISMA) Moderate Certified Amazon Web Services &#39;Infrastructure as a Service&#39; (IaaS) platform.   **Note:** _although the AWS environment is FedRAMP compliant, as a cost-saving measure, systems do not include FedRAMP certifications which are specific to each HIX member&#39;s Virtual Private Cloud (VPC) infrastructure, since the AWS environment already exceeds federal and HIPPA security requirements for HBX._

Our DevOps team of cloud architects, cloud engineers and system administrators ensure high-availability and performance for each HIX Community Member&#39;s Amazon Web Service (AWS) cloud-based infrastructure by deploying across multiple AWS Availability Zones (AZ) within a geographic region. AWS regions each contain three to four Availability Zones.  The strategy of deploying infrastructure across multiple Availability Zones significantly reduces the risk of system downtime due to a catastrophic failure. The DevOps team will also work closely with each HIX Community Member&#39;s Operations and Maintenance (O&amp;M) team to establish connectivity with their data centers.

## Step 2: Prepare Software Development Environment
To support ongoing project needs, coordinated application project development and maintenance environments are hosted using cloud-based virtual machine instances.  Each development environment is comprised of two main components:

1. **Development Workbench** - online tools that manage: a) project documentation; b) software source code version control repository; and c) issue tracking and resolution.
2. **Test Environment** - server instances, which are functionally equivalent to, but physically isolated from, the production environment.  This environment serves two primary purposes: 1) software development testing and staging; and 2) HIX Community stakeholder review of software during development. This test environment may be turned over to the HIX Community Member partner or decommissioned at the end of the project.

DCHBX will configure a coordinated development workbench that organizes and supports the activities related to software development and maintenance.  The development workbench will provide online access and support for project documentation, source code version control repository and issue tracking.

The development workbench is a collaborative environment where HIX Community stakeholders and DCHBX developers access system components as they&#39;re created and improved, enter new requests and issues, and monitor progress on their resolution.

The development workbench includes servers, physically isolated from production servers, for software integration testing and staging. Procedures are defined by the DCHBX AppDev team for committing code to the source code version control repository and code promotion through development -&gt; test -&gt; staging -&gt; production environments.

## Step 3: Define Requirements through Use Cases
At the beginning of each project development iteration, the DCHBX team conducts a kickoff meeting to refine the scope of work, align expectations, confirm roles and responsibilities, and verify contacts who will be involved in the project.

Typically, one or more Joint Application Development (JAD) sessions are held with stakeholders to gain and document user knowledge and gather system requirements in the form of Use Cases.  Use Cases describe system capabilities and behavior from the perspective of stakeholders (Actors) who will use the system in the form of short stories.

Descriptions for these Use Cases will be documented using the DCHBX online Development Workbench referenced in Step 2 above.  At this stage, the documentation defines the following system elements:

* **Actors** – various roles taken by human stakeholders and other computer systems that will interact with the new system
* **Use Cases** – the system supports to satisfy Actor needs
* **Story Points** – relative level of effort necessary to develop the Use Case

Once the Use Cases collected from JAD sessions are documented and reviewed by stakeholders, DCHBX senior project team members host follow-up meetings and teleconferences to assist the stakeholders in prioritizing requirements necessary to arrive at a useful system that:

* Achieves business goals for the development iteration cycle; and
* Is attainable within the allotted time and resource constraints

We recommend the so-called &#39;MoSCoW&#39; method for prioritizing requirements: &quot;Must have&quot;, &quot;Should have&quot;, &quot;Could have&quot;, and &quot;Won&#39;t have&quot;.  Using this method, a finalized, ranked set of Use Cases is presented to the stakeholders for approval to proceed with Use Case elaboration and high-level design for the development iteration.

## Step 4: Elaborate Use Cases, Design System and Data Model
Use Case requirement information, along with proven software design principles, are applied to design the system interface, database and application code components.

Use Case summaries define information necessary to break down development activities into short-duration tasks for assignment to developers. Technical specifications describe trigger events, preconditions, basic and alternative courses of events for each Use Case. This additional level of elaboration provides the basis for designing software components and their interfaces. Other diagrams using unified mark-up language (UML) notation (e.g.; sequence, package diagrams) may be produced where appropriate to communicate system design requirements.

User Interface wire frame designs are prepared, depicting general application layout, navigation and interface components. The wire frame design is reviewed with stakeholders, incorporating comments and feedback.

Once requirements have been reviewed and Use Cases defined, application information models are designed.  These models either draw from and extend existing database designs, or create and implement new database designs as necessary.  The extensions cover new data content and associations with existing data.

## Step 5: Develop and Test Software
System components are developed and tested according to design specifications and artifacts prepared under previous activities.  Our software development strategy is to implement new, and refactor existing functionality in the simplest and most direct way possible without generalizing.

The DCHBX AppDev team takes a proactive, life cycle-long approach to track issues, ensure development of high quality software and improve existing legacy code.  Rather than waiting until development has concluded to begin testing, we build integrity into systems throughout the development process.  Our collaborative issue tracking system, Test Driven Development (TDD) process and stakeholder access to software under development, early and often, combine to deliver a high quality system.

The development workbench introduced in Step 2 above includes an issue tracking system.  The issue tracker manages a workflow to record and resolve bugs and new features identified in production systems.  It also includes features for reporting and filtering these issues, searching and linking similar tasks, triaging reported issues, assigning work to developers, and generating analytical reports such as resource workload and time periods between issue report and resolution.

Each new Use Case feature or legacy system improvement is managed under our TDD approach, which verifies and validates that software components will function as expected.  To ensure that integrity is built into every phase of development, our developers apply what is commonly referred to as the &#39;Red/Green/Refactor&#39; pattern.  Before coding a system function, the developer writes a test case (spec) that describes and validates proper component behavior based on design specifications.  Next, the test is run and fails (a red result), because no functional code has been written yet.  The developer then proceeds with writing code that meets the requirement and re-runs the automated test until it passes with a green result (indicating the code is behaving as expected).  Finally, the working code may require refinement, such as eliminating redundancy using the DRY (_&#39;Don&#39;t Repeat Yourself&#39;_) principle: a refactor result.

Once coding is authored and tested at the unit level, developers deploy the new software into a software test environment shared with other published system modules. There, a comprehensive set of regression tests run automatically, immediately notifying the development team of any errors that &#39;break the build&#39;.

As component features are implemented, they are made available in the test environment for system stakeholders to review, test, and comment.  Beta tests are typically facilitated with stakeholders approximately two weeks prior to scheduled system release.  As part of this process, testing plans are prepared to help guide stakeholders through system interface, indicate expected behavior and exercise software modules.

DCHBX&#39;s Agile methodology combines issue tracking, automated tests, and early system access to build integrity into the system throughout the development lifecycle. This strategy delivers a much higher quality stakeholder experience - from first interaction with alpha-version code to production release - than is available using less sophisticated approaches.  The net effect is early detection and correction of errors, which reduces the frequency and cost of remedial actions and produces higher quality systems as compared to other methods.

## Step 6: Migrate Data into the New System
Extract, Transform, and Load (ETL), shape and filter legacy data and import into system. Finally, the software is released and training provided.
