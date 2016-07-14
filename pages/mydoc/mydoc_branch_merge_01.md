---
title: Branching and Merging Primer
tags:
  - getting_started
keywords: 'release notes, announcements, what''s new, new features'
last_updated: 'July 3, 2016'
summary: >-
  An introduction to the concept of software configuration management including
  information about why configuration management is important, and the various
  branching and merging strategies.
sidebar: mydoc_sidebar
permalink: mydoc_branch_merge_01.html
folder: mydoc
published: true
---

## Introduction
For some reason, software configuration management (SCM) is still a poorly understood concept. Perhaps this is because software configuration management is largely invisible, perceived to be restrictive, or just seen as boring.

I am not sure why, but the fact is that development inefficiencies (and other downstream activities such as operations) are commonly caused by poor implementations of software configuration management practices.
Software configuration management is "[T]he process of identifying and defining the configuration items in a software system, controlling the release, versioning and change of these items through out the software system life cycle, recording and reporting the status of configuration items and change requests, and verifying the completeness and correctness of configuration items." (Source: Infosys)

As you can see, software configuration management in its entirety is a broad topic, so I decided to focus on one specific aspect in this paper—branching and merging. The topic is fundamental, yet poorly understood by many.

This paper explains the concept, not the mechanics, of branching and merging, but is not specific to any particular software configuration management tool.

## Why SCM Is Important
SCM practices provide the foundation that helps all members of a development team collaborate effectively. No one doubts the importance of having a solid foundation to support a high-rise building, but few seem to understand that software configuration management plays a similar role in software development.

I frequently discuss testing or deployment inefficiencies with customers, only to discover that the root cause was poor software configuration management practices such as testing the wrong configuration, using the wrong test environment, deploying a faulty build, and so on. These problems seem to be the norm instead of the exception.

The benefits of good SCM practices include the following:

- Safeguarding intellectual property—the software assets.
- Helping to improve communication among team members.
- Providing a way to establish clear responsibilities and accountabilities.
- Providing traceability and reproducibility.
- Facilitating reusability.
- Providing for consistency, reliability, and integrity.

## Tradeoffs Between Risk and Productivity

A branching and merging strategy involves a tradeoff between risk and productivity. You trade the safety of working in isolation for the increased productivity of working with other people. The productivity increases come with a cost—the additional effort required for merging software assets sometime in the future.
Using branches provides better isolation and control of individual software assets and increases productivity, because teams or individuals can work in parallel. However, using branches also requires an increase in merge activities and therefore risk, because you must later reassemble branches into a whole.
Unfortunately, there is no such thing as a free lunch!

## Branches
When deciding on an SCM strategy, you should first decide what a branch represents. We frequently align branches with system architectures, organizational units, or work breakdown structures (WBS), as summarized in Figure 1.

**Basing a branching strategy on architecture, organization, or work**
![branches]({{site.baseurl}}/mydoctheme/images/IC79488.gif)

## Example of branching Statergies

![]({{site.baseurl}}/mydoctheme/images/branch_types.png)


{% include links.html %}
