---
title: Branching and Merging Primer
tags: [getting_started] [standards]
keywords: Build Standards, version control, source code, sdlc
last_updated: July 3, 2016
summary: "An introduction to the concept of software configuration management including information about why configuration management is important, and the various branching and merging strategies."
sidebar: mydoc_sidebar
permalink: mydoc_branch_merge_01.html
folder: mydoc
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
-Safeguarding intellectual property—the software assets.
-Helping to improve communication among team members.
-Providing a way to establish clear responsibilities and accountabilities.
-Providing traceability and reproducibility.
-Facilitating reusability.
-Providing for consistency, reliability, and integrity.

## Tradeoffs Between Risk and Productivity

I also switched from redcarpet and Pygments to Kramdown and Rouge to align with the current direction of Jekyll 3.0. Kramdown is a Markdown filter (it's slightly different from Github-flavored Markdown). Rouge is a syntax highlighter. Pygments had some dependencies on Python, which made it more cumbersome for Windows users.

## Blog feature

I included a blog feature with this version of the theme. You can write posts and view them through the News link. There's also an archive for blog posts that sorts posts by year.

Additionally, the tagging system works across both the blog and pages, so your tags allow users to move laterally across the site based on topics they're interested in. When you view a tag archive, the sidebar shows a list of tags.

## Updated documentation

I updated the documentation for  the theme. The switch from the multi-site outputs to the single-site with multiple sidebars required updating a lot of different parts of the documentation and code.

## Fixed errors

Previously I had some errors with the HTML that showed up in w3c HTML validator analyses. This caused some small problems in certain browsers or systems less tolerant of the errors. I fixed all of the errors.

## Accessing the old theme

If you want to access the old theme, you can still find it [here](https://github.com/tomjohnson1492/jekylldoctheme-separate-outputs).

{% include links.html %}
