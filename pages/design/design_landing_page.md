---
title: Design Overview
keywords: architecture soa system design
sidebar: design_sidebar
toc: false
permalink: design_landing_page.html
folder: design
---


## Extension

The Enroll Application is purposely designed and applies the following technical patterns for extension and customization at multiple system levels:

* Enterprise Architecture level: the system applies an event-driven service-oriented architecture, where operations are orchestrated between component services, connected via Advanced Message Queuing Protocol middleware, and communicate using a common Canonical Vocabulary, the ACApi.  DCHBX uses this architecture implementation to integrate with COTS and proprietary systems inside the District of Columbia and with contractors.

* Application level: UI presentation and business rule settings that may vary between exchanges (i.e. site name, minimum open enrollment period, qualifying life events, maximum employee retroactive termination) may be setup in site-specific configuration files.

* Code Level: within the application, functions that may have multiple implementations, such as premium credit strategies (i.e. employer fixed cost, percentage contribution, indexed percentage contribution) are designed as pluggable components that may be supported and interchanged, as appropriate.  At a structural level, the Enroll Application’s Ruby on Rails supports RubyGems, a package manager for encapsulating distributing independent programs and code libraries. 

DCHBX will continue to use the current Github code hosting and version control system and proven processes for managing the production code base and development branches.  Custom extensions will use one or more of the above patterns to add functionality to the system.  This model supports coordinated contributions from development teams both internal and external to DCHBX.  

System updates will be distributed to multiple sites and environments using automated deployment, already a common DCHBX practice.

DCHBX’s goal is to establish a sustainable state-based marketplace community that shares a built-to-purpose technology system.  As part of this vision, the community collaborates on managing and maintaining a common core function, with the flexibility to extend and customize system operations to meet individual organization needs.   Custom development may be paid for by one, or cost-shared between multiple, community members.  For example, a significant new feature, that’s useful to multiple marketplaces, may be cost-shared on a voluntary basis.  