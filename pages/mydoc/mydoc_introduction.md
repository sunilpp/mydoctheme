---
title: Build Request Process
tags:
  - best_practices
  - process
  - standards
summary: >-
    Build Request Process , SLA's , important Contacts etc...
sidebar: mydoc_sidebar
permalink: mydoc_introduction.html
folder: mydoc
published: true
---

## Build Request Process

- Any build/Deploy request should be  be notified in advance so that resources can be allocated appropriately.
- Preferably one week advance notice for Production/Customer Staging/DR Environments
- Self service for non prod and Devlopment environment (2 business days in advance for QA if assistance required ,Only 1 request is needed for QA per release)

> We understand that it is hard to determine an exact date.  A ticket can be submitted with an estimated date, we mainly want to know that a release is coming soon.For QA, only one ticket will be required for that release, in the event another build/deployment is needed.  Please e-mail/call the build team with the services/application needed to be built/deployed and reference the current QA OPAS request.

## Workflow :
- OPAS request is created with the release form/Build & Deployment instructions filled in and attached to the ticket.
- Build Team Manager/Lead will review the ticket and approve/assign  if the ticket is complete.
- Build Engineer to perform the build/release.
- Build Engineer to notify the submitter and application team of completion and standby for confirmation from the QA tester.
- If cases of rollback, the Build Engineer will be available to support.
- All issues to be recorded in the release form and the problem list log.
- Once the request has been completed and any issues have been resolved, the ticket will be set to complete.
## Normal Process
 - At least 2 business days advance notice in order to get resources in line to work on request.
 - Resource will be assigned and this will be communicated to requestor within one Business day.
## Emergency Build/Deploy
 - Problem is discovered and needs immediate action - Resource available or on call engineer will take on responsibility of getting everything needed in place and will either take care of the request or will make sure transition information is in place.
 - Release is causing production outage -Available build engineer resource will work on issue or on-call engineer.

## Getting started

To get started, see [Getting Started][index].

{% include links.html %}
