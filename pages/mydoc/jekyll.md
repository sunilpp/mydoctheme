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


## Jekyll 

Jekyll is configured and running on bnrqn1vpcdmst02

## Start jekyll 

```
sudo su – builder
cd /apps/Jekyll/mydoctheme
git clone https://github.com/sunilpp/mydoctheme 
  (we should make it private repo or move it to GitLab .)

bundle install 
bundle exec jekyll serve --host 10.216.41.43 --port 7000
OR 
jekyll serve --host=10.216.41.43 --port=7000

```

make sure you use an unused port, considering we have docker and cjoc services running on this server 


## Add/Modify section in the Sidebar  

[https://github.com/sunilpp/mydoctheme/blob/gh-pages/_data/sidebars/mydoc_sidebar.yml](https://github.com/sunilpp/mydoctheme/blob/gh-pages/_data/sidebars/mydoc_sidebar.yml)

just add the resp section in the YAML  file  .

## Add a new page 

[https://github.com/sunilpp/mydoctheme/tree/gh-pages/pages/mydoc](https://github.com/sunilpp/mydoctheme/tree/gh-pages/pages/mydoc)

create a new file under this location 
make sure to describe the file with this template , or add this to the start of the page  (no spaces at the top )

```
---
title: Apache SuperHost
tags:
  - Build Utilties 
  - Build
  - devops_tools
keywords: null
summary: >-
  THis is regarding the apache superhost for Build Infra.
sidebar: mydoc_sidebar
permalink: apache_superhost.html
folder: mydoc
published: true
---

```

