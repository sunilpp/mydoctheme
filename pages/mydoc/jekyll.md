---
title: Jekyll
tags:
  - build_metrics 
  - Jekyll
  - Documentaion
keywords: null
summary: >-
    Content aware documentaion using jekyll  .
sidebar: mydoc_sidebar
permalink: jekyll.html
folder: mydoc
published: true
---


##Jekyll 

Jekyll is configured and running on bnrqn1vpcdmst02
sudo su – builder
cd /apps/Jekyll/mydoctheme
git clone https://github.com/sunilpp/mydoctheme 
  (we should make it private repo or move it to GitLab .)

bundle install 
bundle exec jekyll serve --host 10.216.41.43 --port 7000
OR 
jekyll serve --host=10.216.41.43 --port=7000

make sure you use an unused port, considering we have docker and cjoc services running on this server 
