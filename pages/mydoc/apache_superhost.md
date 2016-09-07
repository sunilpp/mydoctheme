---
title: Apache SuperHost
tags:
  - Build Utilties 
  - Build
keywords: null
summary: >-
  THis is regarding the apache superhost for Build Infra.
sidebar: mydoc_sidebar
permalink: apache_superhost.html
folder: mydoc
published: true
---

## Adding a new proxy website in Apache  (IP based Virtual Host )

Build Apache in DMZ -  bnrqn1vpasweb01/02  

### Step 1

Request for a new Additional IP in the same range as the current IP’s on the server (10.209.10.XXX)  - raise a ticket  to  Dell networking .

### Step 2.

Plumb the IP to the Server - Dell INTEL team ticket.

### Step 3: Setup the new virtual Host.

Use an example template like build.corelogic.net.conf
Ex :

