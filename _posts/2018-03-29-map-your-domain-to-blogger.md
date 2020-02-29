---
ID: 13
post_title: Map Your Domain to Blogger
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=13
published: true
post_date: 2018-03-29 20:00:46
---
Mapping your domain is an important part of stateu.org; it reinforces the idea that you don't necessarily need to host all your own applications. You should, however, be mindful of making your web presences part of a domain you control. If you would like to map a subdomain and have not yet created it, use&nbsp;<a class="urlextern" title="https://stateu.org/support/cpanel/creating-subdomains" href="http://stateu.org/docs/uncategorized/setting-up-subdomains/" target="_blank" rel="nofollow noopener noreferrer">this tutorial on creating subdomains</a>&nbsp;before proceeding. To map your domain, or a subdomain, to Blogger, use these steps:
<ol>
 	<li class="level1">Log in and navigate to your cPanel. Click the&nbsp;<strong>Search box</strong>&nbsp;at the top, right-hand corner and type “<abbr title="Domain Name System">DNS</abbr>” (without the quotes).</li>
 	<li class="level1">Click on the&nbsp;<strong>Zone Editor</strong>&nbsp;icon.</li>
 	<li class="level1">Find the domain (or subdomain) you want to map to Blogger in the list and click <strong>Manage</strong>.
<div class="li">&nbsp;</div></li>
 	<li class="level0">
<div class="li">Create a new&nbsp;<strong>CNAME</strong> record by clicking <strong>Add Record</strong>. To save, click Add Record.<img class="alignnone size-full wp-image-139" src="https://stateu.org/docs/wp-content/uploads/2018/03/Screen-Shot-2018-03-30-at-3.51.47-PM.png" alt="" width="1380" height="86">Keep this window open; you will need it in later steps.</div></li>
 	<li class="level0">
<div class="li">In a new window, go to the Blogger website, and login with your Blogger/Google username and password.</div></li>
 	<li class="level0">
<div class="li">From your Blogger Dashboard, find the blog you'd like to use, expand the&nbsp;<strong>More Options</strong>&nbsp;menu, and click&nbsp;<strong>Settings</strong>.</div></li>
 	<li class="level0">
<div class="li">On the “Basic Settings” page, find the Publishing section, and click the&nbsp;<strong>Setup a 3rd party&nbsp;<abbr title="Uniform Resource Locator">URL</abbr>&nbsp;for your blog</strong>&nbsp;link.</div></li>
 	<li class="level0">
<div class="li">Under&nbsp;<strong>Advanced Settings</strong>, type the full subdomain or domain you are mapping into the box, leave the&nbsp;<strong>Use missing files host?</strong>&nbsp;option set to&nbsp;<strong>No</strong>, then click&nbsp;<strong>Save</strong>.</div></li>
 	<li class="level0">
<div class="li">You will be presented with a message that your domain cannot be verified, along with information about your existing&nbsp;<abbr title="Domain Name System">DNS</abbr>&nbsp;entry, and an additional&nbsp;<abbr title="Domain Name System">DNS</abbr>&nbsp;entry that needs to be made. This is normal. Copy the second entry under the&nbsp;<strong>Name, Label, or Host entry</strong>&nbsp;to your clipboard.</div></li>
 	<li class="level0">
<div class="li">Go back to the window or tab containing the<strong>&nbsp;Zone Editor</strong>&nbsp;in your StateU cPanel. Create another records&nbsp;by clicking&nbsp;<strong>Add a Record</strong>. Paste the text you just copied into the&nbsp;<strong>Name</strong>&nbsp;field. This information will be different for each domain. Set the&nbsp;<strong>TTL</strong>&nbsp;field to 14400, and the&nbsp;<strong>Type</strong>&nbsp;drop-down menu to&nbsp;<strong>CNAME</strong>.&nbsp;<img class="mediacenter" src="https://stateu.org/docs/wp-content/uploads/2019/10/edit_blogger_record_final_1.png" alt=""></div></li>
</ol>
<ol>
 	<li class="level0">
<div class="li">Go back to the window or tab containing the Blogger Advanced settings panel, and copy the second entry under the&nbsp;<strong>Destination, Target, or Points to</strong>&nbsp;column to your clipboard.</div></li>
 	<li class="level0">
<div class="li">Go back to the window or tab containing the&nbsp;<strong>Advanced&nbsp;<abbr title="Domain Name System">DNS</abbr>&nbsp;Zone Editor</strong>&nbsp;in your stateu.org cPanel. In the&nbsp;<strong>Zone File Records</strong>&nbsp;section, find the domain you were editing&nbsp;<strong>Action</strong>&nbsp;for and paste the text you just copied into the&nbsp;<strong>CNAME</strong>&nbsp;field. This information will be different for each domain. Click&nbsp;<strong>Add record&nbsp;</strong>when you are done.</div></li>
 	<li class="level0">
<div class="li">Return to the window or tab containing the Blogger Advanced settings panel, and click&nbsp;<strong>Save</strong>.</div></li>
 	<li class="level0">
<div class="li">If everything was successful, your domain will now appear as the&nbsp;<strong>Blog Address</strong>. Keep in mind that it may take up to 72 hours for your domain or subdomain to correctly point all visitors to the correct location.</div></li>
</ol>
For further instructions, click <a href="http://www.bloggerplugins.org/2015/01/how-to-setup-custom-domain-on-blogger-with-godaddy-com.html" target="_blank" rel="noopener noreferrer">here</a>.