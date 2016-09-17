---
title: Managing Infrastructure
keywords: software development lifecycle sdlc DevOps infrastructure cloud
sidebar: dpb_sidebar
toc: false
permalink: dpb_managing_infrastructure.html
folder: playbook
---
## Managing Infrastructure

The DCHBX team&#39;s Agile methodology and [Lean](http://www.poppendieck.com/) development practices are not limited to software development.  Our highly skilled DevOps engineers are proficient in the most up-to-date cloud and data center infrastructure design and operations best practices.  The DCHBX customized Enroll Application solution provides HIX Community Member partners with flexible and secure infrastructure designs to host their applications in the cloud.  Our engineers have adopted an &#39;Infrastructure as Code&#39; (IaC) approach to DevOps, which in many ways, parallels our software development practices.  Infrastructure as Code provides our DevOps engineers with the ability to apply tools such as version control systems (VCS), continuous integration (CI), logging, monitoring, automated testing environments, auto-scaling based on traffic load, backup, and real-time performance and error monitoring/recovery.  In mission-critical operations where downtime of any duration is not acceptable (such as a state-based health insurance marketplace), Infrastructure as Code enables automated software deployment with zero downtime using Chef, Capistrano and other related tools.

The IaC approach has been &#39;battle-proven&#39; in the toughest and most demanding IT environments in the industry such as: Amazon, Google, Netfilx and Facebook.

This approach to managing infrastructure targets goals which parallel those of our Agile software development methods:

* Anticipate that requirements will change over time
* Deployments, upgrades and other system enhancements become routine, absent of the drama and system disruption traditionally experienced
* Enables DevOps engineers to be productive and deliver value, instead of performing routine and repetitive tasks
* Provides DevOps teams with the ability to recover quickly when things do not go as planned

Once cloud environments have been established and successfully deployed for a new system, DevOps configures the necessary managed services referenced above.  As part of the system standup process, a Disaster Recovery (DR) environment is established and maintained in a separate AWS geographic region to enable recovery in the case of catastrophic failure in the primary operation region.

Combining our Agile software development methods with Infrastructure as Code helps to eliminate uncertainty and restore predictability to technology development processes and system operations.

![AWS Architecture](/images/enroll_app_aws_logical_architecture.png)
