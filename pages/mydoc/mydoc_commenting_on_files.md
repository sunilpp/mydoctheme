---
title: CoreLogic Escrow Tax Services
tags:
  - navigation
keywords: "annotations, comments, feedback"
last_updated: "November 30, 2016"
summary: "You can add a button to your pages that allows people to add comments."
sidebar: mydoc_sidebar
permalink: mydoc_commenting_on_files.html
folder: mydoc
---

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a class="noCrossRef" href="#about" data-toggle="tab">About</a></li>
    <li><a class="noCrossRef" href="#migrateWindow" data-toggle="tab">Migration Window</a></li>
    <li><a class="noCrossRef" href="#contact" data-toggle="tab">DEV Team Contact</a></li>
</ul>
  <div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="about">
    <h2>About</h2>
<p>Praesent sit amet fermentum leo. Aliquam feugiat, nibh in u ltrices mattis, felis ipsum venenatis metus, vel vehicula libero mauris a enim. Sed placerat est ac lectus vestibulum tempor. Quisque ut condimentum massa. Proin venenatis leo id urna cursus blandit. Vivamus sit amet hendrerit metus.</p>
</div>

<div role="tabpanel" class="tab-pane" id="migratewindow">
    <h2>Migration Windows</h2>
   <table border="0" class="bodyTable">
<tbody><tr class="a">
<td align="center">Region</td>
<td align="center">UTC</td>
<td align="center">1hr</td>
<td align="center">1hr</td>
<td align="center">2hr</td>
<td align="left">1hr</td></tr>
<tr class="b">
<td align="left">US</td>
<td align="left">GMT-6</td>
<td align="left">0800-0900</td>
<td align="left">1200-1300</td>
<td align="left">1700-1900</td>
<td align="left">0030-0130</td></tr>
<tr class="a">
<td align="left">Poland</td>
<td align="left">GMT+1</td>
<td align="left">1500-1600</td>
<td align="left">1900-2000</td>
<td align="left">0000-0200</td>
<td align="left">0730-0830</td></tr>
<tr class="b">
<td align="left">India</td>
<td align="left">GMT+5.30</td>
<td align="left">1830-1930</td>
<td align="left">2230-2330</td>
<td align="left">0330-0530</td>
<td align="left">1030-1130</td></tr>
<tr class="a">
<td align="left">India</td>
<td align="left">GMT+5.30</td>
<td align="left">1930-2030</td>
<td align="left">2330-0030</td>
<td align="left">0430-0630</td>
<td align="left">1200-1300</td></tr></tbody></table>
   </div>

<div role="tabpanel" class="tab-pane" id="contact">
    <h2>Dev Team Contact</h2>
    <p>Vel vehicula libero mauris a enim. Sed placerat est ac lectus vestibulum tempor. Quisque ut condimentum massa. Proin venenatis leo id urna cursus blandit. Vivamus sit amet hendrerit metus.</p>
</div>
</div>

## Java Application Build –EAR/WAR

TAX’s Weblogic Ecosystem contains multiple Clusters per environment and then replicated across all environments, the 160+ applications in scope for TAX Delegate Migration are logically grouped and run on various clusters part of the Weblogic servers.
[knowit.corelogic.net](http://knowit.corelogic.net/doku.php?id=dcm:dcm-adminconsoles)

While using Delegate , Deployment on various Weblogic environments was done using individual shell scripts specific to each environment and the procedure was to copy the WAR/Portlet files between Environments (Dev > Test > Stage > Prod) and then trigger a Restart Cluster using Server specific shell scripts.

Post the completion of this project, Weblogic Deployments will be handled by a single generic perl script which has been configured to toggle between all environments as part of TAX Business Unit. The new script uses WLST to deploy applications and uses another generic script to handle Cluster Restarts. Also, the restart has been improved to do rolling restarts instead of the full restart which old shell scripts were using. This ensures zero down time on the cluster even during the deployment



{% raw %}
```
/apps/home/builder/tax/bin/wl-deploy.pl <GroupID> <ArtifactID> <Version> <Cluster> <Restart Required?> <Workspace>  <WLEnv> <Env> <Apptype(EAR/WAR/Portlet)> <ManagedServers>  

```
{% endraw %}




## TAX Weblogic Deployment Architecture


If you want people to collaborate on your project so that their edits get committed to a branch on your project, you need to add them as collaborators. For your Github repo, click **Settings** and add the collaborators on the Collaborators tab using their Github usernames.

If you don't want to allow anyone to commit to your Github branch, don't add the reviewers as collaborators. When someone makes an edit, Github will fork the theme. The person's edit then will appear as a pull request to your repo. You can then choose to merge the change indicated in the pull or not.

{% include note.html content="When you process pull requests, you have to accept everything or nothing. You can't pick and choose which changes you'll merge. Therefore you'll probably want to edit the branch you're planning to merge or ask the contributor to make some changes to the fork before processing the pull request." %}


## Workflow

Users will make edits in your "reviews" branch (or whatever you want to call it). You can then commit those edits as you make updates.

When you're finished making all updates in the branch, you can merge the branch into the master.

Note that if you're making updates online, those updates will be out of sync with any local edits.

{% include warning.html content="Don't make edits both online using Github's browser-based interface AND offline on your local machine using your local tools. When you try to push from your local, you'll likely get a merge conflict error. Instead, make sure you do a pull and update on your local after making any edits online." %}

## Prose.io

 Prose.io is an overlay on Github that would allow people to make comments in an easier interface. If you simply go to [prose.io](http://prose.io), it asks to authorize your Github account, and so it will read files directly from Github but in the Prose.io interface.

 {% include links.html %}
