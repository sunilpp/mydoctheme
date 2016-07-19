---
title: 'Welcome to the DevOps Enterprise B&R Portal '
keywords: sample homepage
tags:
  - getting_started
sidebar: mydoc_sidebar
permalink: index.html
summary: >-
  This site is intended to help all the developers on the team by providing  an
  overview of the process and standards followed and regarding the tools and
  frameworks used to implement the services/solutions . 
published: true
toc: false
folder: mydoc
---

<a href="{{ site.github.repository_url }}/tree/gh-pages/{{ page.relative_path }}">Edit this page in Github</a>

<div class="row">
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-tree fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Product Lines</h4>
                     <p>Build/Deploy Documentation</p>
                     <a href="tag_product_lines.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-car fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>DevOps Tools</h4>
                     <p>Build/DevOps Tools and platforms</p>
                     <a href="tag_devops_tools.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-support fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Build Standards</h4>
                     <p>Build/DevOps Process and Best Practices</p>
                     <a href="tag_best_practices.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-database fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Build Metrics</h4>
                     <p>Detailed Build Metrics for all products</p>
                     <a href="tag_build_metrics.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
</div>


## Services

- Software Builds & Code Deployments
- Jenkins/QuickBuild CI/CD Setup
- Create/Test/Maintain Automated Build/Deployment scripts
- Build Artifacts Management
- User Mgmt on DevOps Tools and Platforms
- Appstore – Mobile builds
- Sonar – Code Quality Analysis

## Build Request Process

- A notification must be given to the build team in advance so that resources can be allocated appropriately.
- 1 week advance for Production/Customer Staging/DR.
- Self service for non prod and Devlopment environment (2 business days in advance for QA if assistance required ,Only 1 request is needed for QA per release)
- 
   {% include note.html content="We understand that it is hard to determine an exact date.  A ticket can be submitted with an estimated date, we mainly want to know that a release is coming soon.For QA, only one ticket will be required for that release, in the event another build/deployment is needed.  Please e-mail/call the build team with the services/application needed to be built/deployed and reference the current QA OPAS request." %}

## B&R Workflow
- OPAS request is created with the release form/Build & Deployment instructions filled in and attached to the ticket.
- Build Team Manager/Lead will review the ticket and approve/assign  if the ticket is complete.
- The Build Engineer will perform the build/release.
- The Build Engineer will notify the submitter and application team of completion and standby for confirmation from the QA tester.
- If there are any issues or if a rollback is required, the Build Engineer will be available to support.
- All issues will be recorded in the release form and the problem list log.
- Once the request has been completed and any issues have been resolved, the ticket will be set to complete.

## Normal Process
 - At least 2 business days advance notice in order to get resources in line to work on request.
 - Resource will be assigned and this will be communicated to requestor within one Business day.
 
## Emergency Build/Deploy
 - Problem is discovered and needs immediate action - Resource available or on call engineer will take on responsibility of getting everything needed in place and will either take care of the request or will make sure transition information is in place.
 - Release is causing production outage -Available build engineer resource will work on issue or on-call engineer.

{% include links.html %}
