---
ID: 239
post_title: Managing Permissions
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=239
published: true
post_date: 2018-04-03 17:32:50
---
The default Mediawiki installed has been customized to make it a bit harder for spammers to overwhelm wikis with illegitimate content and comments. This is done by modifying the <strong>LocalSettings.php</strong> file (a file that is included in every install in which it is possible to provide configurations details).

By default, Mediawiki allows anonymous users to create pages and edit pages in the wiki. The modifications change this in the following ways:
<ul>
 	<li class="level1">
<div class="li">Anonymous users cannot edit existing pages</div></li>
 	<li class="level1">
<div class="li">Anonymous users cannot create pages</div></li>
 	<li class="level1">
<div class="li">Registered users must click the confirmation link in the registration email in order to edit or create pages</div></li>
</ul>
This approach should drastically reduce unsolicited content and comments on Mediawiki installations. One further step that administrator might take is to turn registration off after a predetermined amount of time. Users must create accounts by this date; after that, the settings are changed so that registrations are no longer open.

To add this setting, you must edit <strong>LocalSettings.php</strong> in your Mediawiki install:
<ol>
 	<li class="vspace">Login to cPanel and browse to your <a class="urlextern" title="https://stateu.org/support/cpanel/accessing-your-files-through-the-file-manager" href="https://stateu.org/docs/uncategorized/accessing-your-files-through-the-file-manager/" target="_blank" rel="nofollow noopener noreferrer">File Manager</a>.
<img class="alignnone size-full wp-image-114" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-03-30-at-12.37-PM.png" alt="" width="759" height="379" /></li>
 	<li class="vspace">In the File Manager, browse to the folder within<strong> public_html</strong> that contains your Mediawiki install. If you installed the wiki at the root of your domain, you won't need to go any further than public_html. If you installed the wiki in a subdomain or subdirectory, you'll need to find the directory that is associated with that space.</li>
 	<li class="vspace">Locate <strong>LocalSettings.php. </strong>Once selecting the file, click <strong>download</strong> in the top menu bar to download the file as a backup before proceeding. Then click <strong>Edit</strong> in the top menu bar to edit the file.
<img class="alignnone size-full wp-image-241" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-03-at-1.21-PM.png" alt="" width="1430" height="727" /></li>
 	<li class="vspace"> Confirm that you want to edit the file.
<img class="shadow alignnone wp-image-465 size-full" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/2019104.4-MediaWiki-files-confirm-edit.gif" alt="Confirm that you want to edit the file" width="502" height="349" /></li>
 	<li class="vspace">Browse to the bottom of the document, and locate the custom settings that were added during the Mediawiki install and the following line:</li>
</ol>
<pre>$wgGroupPermissions['*']['createaccount'] = false;</pre>
<img class="alignnone size-full wp-image-242" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-03-at-1.30-PM.png" alt="" width="743" height="634" />