---
title: DevOps Overview
keywords: devops operations maintenance
sidebar: ops_sidebar
toc: false
permalink: ops_landing_page.html
folder: ops
---
To operate and maintain the system infrastructure, IdeaCrew uses the DevOps model, where the operations and development teams work closely and collaboratively.  Under DevOps, service delivery encompasses the application and infrastructure interaction as a whole, rather than developers concerned only with creating the software, and system engineers responsible for the entire system–software and platform–following release. 

## Lean Processes

DevOps applies Agile software development’s concepts and lean processes to building and managing the infrastructure platform.  Following is an overview of how DevOps functions:

### Server Provisioning

DevOps use AWS command line scripts to initialize and stand up VMs to the Operating System (OS) level.  For each instance kind, these scripts include provisioning parameters that allocate system resources appropriate for the intended server role, including: vCPU count, memory size, storage volumes and capacities, and network subnet.

### Application Configuration

DevOps develops and maintains Chef cookbooks with recipes that install and configure built-to-purpose servers provisioned under the process above.  Examples of server kinds include: http, application, database and logging servers.  The recipes create accounts, folders and services, and install dependencies, such as libraries, packages, and executables.  The results are servers ready to support the intended services. 

### Real Time Auto-scaling

A key benefit of cloud computing is the ability to scale system capacity up and down to meet customer demands.  In this implementation, the application and Web servers for the Enroll Application are configured to launch additional instances when key resource thresholds are exceeded, including CPU and memory utilization maximums.  Within two minutes of the signal to launch, the additional VMs typically are online and handling service load.  These additional instances remain active until the demand levels drop below specified threshold values for a certain time interval (measured in minutes).

### Instrumentation and Monitoring

At the VM level, AWS CloudWatch monitors server and service health, checking VM heartbeat and verifying key services are always running.  If any issues are detected, DevOps personnel are signaled immediately via text message and email.

At both the OS and application level, all log events are forwarded to a central enterprise logging subsystem, using Graylog and the Elasticsearch stack.  At five minute intervals, a process scans the Graylog server looking for application-level notifications and errors, sending notices to DevOps team members over the Slack messaging services.  Additionally, for critical errors, the process automatically opens an issue in the software development ticketing system. 

At the application level, performance is monitored continuously using New Relic.  Client agents are integrated within the Enroll Application software, and report low-level performance indicators, including: CPU, thread and memory usage and efficiency on an application instance level. 

## DevOps Tools

The DevOps team uses the following tools:

* Amazon Web Services (AWS) – secure cloud services platform
* Github – code hosting platform for version control and collaboration
* Chef – configuration management tool for provisioning and building Virtual Machines (VMs)
* Jenkins – continuous integration software tool 
* New Relic – software analytics tool that provides real time performance analytics 
* Graylog – log management and analysis tool
* Slack – real time messaging application for teams

These tools support server provisioning, application configuration, real time auto-scaling, instrumentation and monitoring functions.  Following are examples of how the DevOps team applies these tools to drive a lean, highly efficient infrastructure management model.  
