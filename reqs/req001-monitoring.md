**System Requirements #:** 1  
**Status:** draft  
**Date:** 2014-Dec-28  
**Revision Number:** 1.0  
**Author(s):** Aaron Russo <arusso@berkeley.edu>  
**Reviewer(s):**  
**Approver(s):**  

---

Monitoring System for Platforms & Infrastructure
================================================

Executive Summary
-----------------

Create a monitoring system that provides real time alerting of issues,
capability to be highly automated and provides an improved customer facing
experience.

Goals
-----

*Optional Requirements should be prepended with an '(O)'*
* API access for automation by systems team and customers alike
  * RBAC support to allow customers access without compromising on security
  * Ability to add and remove systems
  * Ability to check status of checks on each system
  * Ability to silence or acknowledge alerts
* Capable of monitoring modern Linux based systems (RHEL5+/2.6.18+)
* Capable of monitoring modern Windows based systems (Win 2k8+)
* Capable of monitoring network devices and appliances via SNMPv2 **AND** SNMPv3
* Capable of receiving SNMP traps
* Templates for quickly provisioning new systems to be monitored
* Tunable alerting thresholds down to the check level
* Flexible alerting system that can integrate with external tools such as
  xMatters and Twilio
* (O) metric collection and graphing
* (O) customized maps or images to help show the entire state of a
  particular system. For example, [nagvis](http://www.nagvis.org/) or
  [RealOpInsight](http://realopinsight.com/).

Non-goals
---------

* An all-in-one system for metric and alerting. If the metrics and graphing
  are built-in and do not take away from the alerting and monitoring features of
  the system it should be considered, but not a requirement for the system.

Background
----------

The environment our current solutions were designed for have changed radically.
We have gone from managing a few, large systems to managing many, smaller
systems built on top of a virtualization platform.

From an organizational perspective, the Unix and Windows teams were at one time
distinct groups that created solutions independantly, without thought to the
others requirement.

With the teams now merged into a single group, and with increasing cooperation
and coordination within the group, we are increasingly finding examples of where
a single system of reference for all aspects of monitoring 

High Level Design
-----------------

*a brief, high-level description of the design; diagrams are helpful*

Detailed Design
---------------

*the design in detail; usually a top-down description*

Alternatives Considered
-----------------------

*alternatives considered and rejected; include pros and cons of each*

Security Concerns
-----------------

*security and privacy ramifications and how those concerns are mitigated*
