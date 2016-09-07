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

## Adding a new proxy website in Apache  (IP based Virtual Host )

Build Apache in DMZ -  bnrqn1vpasweb01/02  

### Step 1

Request for a new Additional IP in the same range as the current IP’s on the server (10.209.10.XXX)  - raise a ticket  to  Dell networking .

### Step 2.

Plumb the IP to the Server - Dell INTEL team ticket.

### Step 3: Setup the new virtual Host.

Use an example template like build.corelogic.net.conf
Ex :

```
Listen  10.209.10.16:443
<VirtualHost 10.209.10.16:443>
    DocumentRoot "/apps/WWW/build.corelogic.net/htdocs"
    ServerName build.corelogic.net
    ServerAdmin cws@corelogic.com
    RewriteEngine on
    RewriteOptions Inherit

   ProxyPass         / http://10.216.2.77:7081/ connectiontimeout=300 timeout=300
    ProxyPassReverse  / http://10.216.2.77:7081/

```

Also make sure the firewalls are open from the apache to the master server CDMSTXX

### Step 4:

 Request for a VIP   with the Apache IP’s as the pool members  , port as 80 and 443  , LB Algorithm  - least used  . – Dell networking and firewall team  .

### Step 5 :

 Add a DNS record for the VIP IP.


