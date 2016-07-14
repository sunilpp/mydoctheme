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

Deciding on the best branching strategy is a balancing act. You must trade off productivity gains against increased risk. One way to validate a chosen strategy is to consider a scenario of change. For example, if you decide to align branches with the system architecture (for example, a branch represents a system component) and you expect significant architectural changes, you might have to restructure your branches and associated processes and policies with each change. Choosing an inadequate branching strategy can cause process overheads and lengthy integration and release cycles that prove frustrating for the whole team.

## Common Branching Strategies
_This section outlines common branching strategies. The intention is not to provide specific guidance, but to stimulate ideas and demonstrate the importance of carefully planning your branching strategy._

### Branch per Release

One of the most common branching strategies is to align branches with product releases, as shown in Figure 2. A branch holds all the software development assets for a single release. Occasionally, you must merge updates from one release to another, but they usually never merge. You discontinue a branch when you discontinue its release.

![]({{site.baseurl}}/mydoctheme/images/branch-1.gif)

### Code-Promotion Branches
Another very common approach is to align branches with software asset promotion levels, as shown in Figure 3. A specific development version is branched off into a Test branch, at which all the integration and system testing is performed. When you complete testing, the software development assets are branched into the Production branch and ultimately deployed.

![]({{site.baseurl}}/mydoctheme/images/branch-2.gif)

During the testing effort, you update the development code base as you find and fix bugs. You merge the changed code into the Development branch when you promote the tested code into production.

## Branch per Task

To avoid overlapping tasks (or activities) and a loss in productivity, you can isolate a task on a separate branch, as shown in Figure 4. These branches should be short-term branches that you merge as soon as you complete the task; otherwise, the merging effort required might exceed the productivity benefits of creating a separate branch for a task.

![]({{site.baseurl}}/mydoctheme/images/branch-3.gif)

### Branch per Component
You could align each branch with the system architecture as shown in Figure 5. In this strategy, you branch off individual components (or subsystems). Then each team developing a component decides when to merge their code back into the development line that serves as the integration branch.

![]({{site.baseurl}}/mydoctheme/images/branch-4.gif)

This strategy can work well if system architecture is in place and the individual components have well-defined interfaces. The fact that you develop components on branches enables more fine-grained control over software development assets.

### Branch per Technology
Figure 6 shows another branching strategy aligned with the system architecture. Here you align the branches to technology platforms. Common code is managed on a separate branch.
![]({{site.baseurl}}/mydoctheme/images/branch-5.gif)

Because of the unique nature of the software development assets managed on the branches, you will probably never merge the branches.

There are many other options for structuring branches, but I hope it is obvious by now that planning the implementation of a branching strategy is worthwhile and can return significant benefits.

## Branching and Merging Anti-Patterns

You know you are on the wrong track if you experience one or more of the following symptoms in your development environment:

- Merge Paranoia—avoiding merging at all cost, usually because of a fear of the consequences.
- Merge Mania—spending too much time merging software assets instead of developing them.
- Big Bang Merge—deferring branch merging to the end of the development effort and attempting to merge all branches simultaneously.
- Never-Ending Merge—continuous merging activity because there is always more to merge.
- Wrong-Way Merge—merging a software asset version with an earlier version.
- Branch Mania—creating many branches for no apparent reason.
- Cascading Branches—branching but never merging back to the main line.
- Mysterious Branches—branching for no apparent reason.
- Temporary Branches—branching for changing reasons, so the branch becomes a permanent temporary workspace.
- Volatile Branches—branching with unstable software assets shared by other branches or merged into another branch.



{% include links.html %}
