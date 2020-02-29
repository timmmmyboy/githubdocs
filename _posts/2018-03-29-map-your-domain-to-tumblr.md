---
ID: 14
post_title: Map Your Domain to Tumblr
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=14
published: true
post_date: 2018-03-29 20:00:46
---
Mapping your domain is an important part of stateu.org; it reinforces the idea that you don't necessarily need to host all your own applications. You should, however, be mindful of making your web presences part of a domain you control. If you would like to map a subdomain and have not yet created it, use <a class="urlextern" title="https://stateu.org/support/cpanel/creating-subdomains" href="http://stateu.org/docs/uncategorized/setting-up-subdomains/" target="_blank" rel="nofollow noopener noreferrer">this tutorial on creating subdomains</a> before proceeding. To map your domain, or a subdomain, to Tumblr, use these steps:
<ol>
 	<li>Log in and navigate to your cPanel. Click the <strong>Search box</strong> at the top, right-hand corner and type “<abbr title="Domain Name System">DNS</abbr>” (without the quotes). As you type, the cPanel page will begin to narrow down results.</li>
 	<li>Find and click on <strong>Zone Editor</strong> to continue.</li>
 	<li class="level0">
<div class="li">Find the domain, or subdomain, you want to map to Tumblr in the list of <strong>Zone File Records</strong>. Click <strong>Manage</strong> next to the proper domain.</div></li>
 	<li class="level0">
<div class="li">Leave the Name, and TTL fields set to their defaults. Update the <strong>Type</strong> drop-down menu to <strong>CNAME</strong>, and the <strong>Address</strong> field to <strong>domains.tumblr.com</strong>. Click <strong>Edit Record</strong> when you are done.</div></li>
 	<li class="level0">
<div class="li">Visit the Tumblr website, and login with your Tumblr username and password.</div></li>
 	<li class="level0">
<div class="li">After logging in, click the Tumblr <strong>Settings</strong> icon.</div></li>
 	<li class="level0">
<div class="li">For the Tumblog you'd like to use under the <strong>Username</strong> click the pencil icon to edit these settings.</div></li>
 	<li class="level0">
<div class="li">Check the <strong>Use a custom domain</strong> checkbox. Type the name of the domain or subdomain you want to map to Tumblr into the box, then click <strong>Test your domain</strong>.</div></li>
 	<li class="level0">
<div class="li">If your domain mapping was successful, you'll see a message that your domain is now pointing to Tumblr. Click the <strong>Save</strong> button before leaving the page. Keep in mind that it may take up to 72 hours for your domain or subdomain to correctly point all visitors to the correct location.</div></li>
</ol>