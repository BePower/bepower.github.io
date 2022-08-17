---
layout: default
title: Hubject
nav_order: 2
parent: Operations
grand_parent: Roaming
permalink: /docs/roaming/operations/hubject
---

# Interoperability via Hubject
{: .no_toc }

Operations procedures for Hubject interoperabilities
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{: toc }

---

## OPERATING PROCEDURES

### Interoperability with BE CHARGE as Mobility Service Provider

The Charging Point Operator (from now on, the "CPO") confirms to have the following requirements:

- The CPO provides the MSP with a I level support reachable by phone (24/7, EN).

- The CPO provides the MSP with a backoffice e-mail (business hours, EN).

- The CPO provides the MSP with e-mail and telephone contacts of at least one reference person with operational skills.

Moreover, the CPO does agree to:

- Implement the operational procedures as presented in this document.

- Fill in the contact form on the interoperability platform with all the information above.

- Schedule a KOM within 5 business days, if required by the MSP, in case of new operating procedures to be implemented.

### Definition of workflow / decision management issue

MSP thanks to its Call Center provides support to MSP's users (from now on, the "User").

Standard engagement with CPO Call Center (from now on, the "CPOcc"), limited to very specific cases, requires the User to call MSP Call Center (from now on, the "MSPcc") and that the latter contacts CPOcc at the phone number provided in the CPO contact form on the interoperability platform.

Once in contact, MSPcc will confirm the User's identity to CPOcc in a unique way through the exchange between Call Center operators of the User's token id and EVSE label asking for support and explaining the issue occurring.

The only cases when MSPcc and CPOcc are asked to be in direct contact are the following:

- The User notifies MSPcc a cable unlocking failure or finishing charging issue.

  - If the User is unable to end the charging session, unlock the charging cable from the EVC or free the EV from the EVC following the standard procedures, MSPcc will contact CPOcc asking them to perform an Unlock command on the specified EVSE while keeping in touch with the User.

    - In case of successful outcome, no other action is required.

    - In case of unsuccessful outcome, if the user authorized the MSPcc to give his telephone contact, the CPOcc, informed by MSPcc, will contact the User and put in place what is necessary to solve the problem.

  - In case all the actions taken by the CPOcc do not allow the resolution of the problem occurred (e.g. the charging cable cannot be released) the CPO will schedule on-field intervention.

  - The outcome of the support will be immediately notified by the CPOcc to the MSP:

    - In case of successful outcome by writing an email to MSP support and to focal points as provided in the contact form on interoperability platform.

    - In case of unsuccessful outcome by both 1) informing MSPcc at the phone number provided in the contact form on interoperability platform and 2) writing an email to MSP support and to MSP focal points as provided in the contact form on interoperability platform.

- The User notifies MSPcc that an EVC managed by CPO presents a situation of danger or missing safety. MSPcc notifies CPOcc with EVSE label and/or EVC address asking for prompt intervention.

Any request for support or investigation originating by either MSP or CPO which does not fall into the previous cases and therefore does not require immediate resolution, must be handled between MSP and CPO via e-mail as provided in the CPO contact form on Hubject platform and using the template of communication as provided in point 2.

Any deviations from the standard procedure, such as MSP users directly calling CPOcc (e.g. CPO phone number printed on the EVC) will be managed as follows:

- The User notifies CPOcc a cable unlocking failure or finishing charging issue. CPOcc will ask the User some questions regarding operational information (e.g. at what time the charging session started, which is the EVSE label, which is the EVC address). If the answers are consistent with what is shown on the CPO backend, CPOcc will provide assistance to the User. Otherwise, CPOcc will suggest the User to contact MSPcc.

- The User notifies CPOcc that he is unable to start a charging session from MSP APP or using MSP RFID card. CPOcc will suggest the User to contact MSPcc.

- The User notifies CPOcc that CPO's EVC is out of order or does not allow charging or has been damaged. CPOcc will follow internal procedure to solve the issue. CPOcc will suggest the User to search for another charging station using MSP APP if a charging transaction is required.

- In all other cases: CPOcc will suggest the User to contact MSPcc.

### Template of communication via email

The following communication template contains the minimum set of information that needs to be shared to allow correct troubleshooting of any event/issue.

| Date and time | Date and time expressed in UTC when the event occurred in the format dd/mm/yyyy hh:mm (whenever the exact time is not available, an indicative time is useful for troubleshooting) |
| EVSE id       | EVSE where the event/issue occurred              |
| Token         | Token affected by the event/issue                |
| CDR id        | Charging Data Record affected by the event/issue |
| Event         | Brief description of the event/issue             |
