---
ID: 20
post_title: Setting Up FTP
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=20
published: true
post_date: 2018-03-29 20:00:46
---
<div class="level1">

There may be times when you need to upload files to your website in the State University web hosting environment. There are a number of scenarios when this might be necessary:
<ul>
 	<li class="level1">
<div class="li">You're working with an application that allows you to install plugins/extensions, but the files need to be manually added to your file manager in order to install them. (Note: This is <em>not</em> required for WordPress which allows you to install themes/plugins through the WordPress dashboard.)</div></li>
 	<li class="level1">
<div class="li">You've developed a custom site/pages using a Web design program, and you need to upload the files you created to your file manager</div></li>
 	<li class="level1">
<div class="li">You're installing an application that isn't part of <a class="wikilink1" title="cpanel:applications-available-in-installatron" href="https://stateu.org/docs/uncategorized/installing-applications-with-installatron/" target="_blank" rel="noopener noreferrer">applications list in Installatron</a>.</div></li>
</ul>
One way to upload files is by using <a class="wikilink1" title="cpanel:accessing-your-files-through-the-file-manager" href="https://stateu.org/docs/uncategorized/accessing-your-files-through-the-file-manager/" target="_blank" rel="noopener noreferrer">the File Manager</a> that is part of <a class="wikilink1" title="cpanel:introduction-to-cpanel" href="https://stateu.org/docs/uncategorized/introduction-to-cpanel/" target="_blank" rel="noopener noreferrer">cPanel</a>. However, sometimes you'll find it easier/necessary to use File Transfer Protocol (FTP) to move files to your site. This can be particularly useful if you're working with a Web space where you're not the owner (so you don't have access to the File Manager in cPanel) or if you need to provide file access to someone else to your space on the Web server. File Manager also only allows you to upload files one by one, so if you're working with large amounts of data then FTP will be preferable.

</div>
<h2 id="what-exactly-is-ftp" class="sectionedit2">What exactly is FTP?</h2>
<div class="level2">

File Transfer Protocol is a method that allows you to remotely move files to a Web server from another location – usually your local/personal computer. Using a pre-defined <abbr title="File Transfer Protocol">FTP</abbr> account (with a username and password), you can configure an <abbr title="File Transfer Protocol">FTP</abbr> client (a program you run on your computer that allows you to transfer files via <abbr title="File Transfer Protocol">FTP</abbr>.

There are lots of <abbr title="File Transfer Protocol">FTP</abbr> clients that you can use; some are free and some are not. A few free ones you might consider:
<ul>
 	<li class="level1">
<div class="li"><a class="urlextern" title="https://filezilla-project.org/" href="https://filezilla-project.org/" target="_blank" rel="nofollow noopener noreferrer">FileZilla (Mac &amp; PC)</a></div></li>
 	<li class="level1">
<div class="li"><a class="urlextern" title="http://cyberduck.io/" href="http://cyberduck.io/" target="_blank" rel="nofollow noopener noreferrer">CyberDuck (Mac &amp; PC)</a></div></li>
</ul>
For the purpose of this tutorial, we'll show you how to set up <abbr title="File Transfer Protocol">FTP</abbr> in FileZilla, (Cyberduck instructions can be found <a href="https://community.reclaimhosting.com/t/ftp-file-transfer-protocol/304" target="_blank" rel="noopener noreferrer">here</a>) but you should be able to generalize these instructions to use in any <abbr title="File Transfer Protocol">FTP</abbr> client.

</div>
<h2 id="get-information-about-your-ftp-account" class="sectionedit3">Get Information about Your FTP Account</h2>
<div class="level2">

If you're connecting via FTP to your own space on State University, or if you're setting up an <abbr title="File Transfer Protocol">FTP</abbr> account for someone else to use, you'll need to start by getting the proper <abbr title="File Transfer Protocol">FTP</abbr> credentials from cPanel:
<ol>
 	<li class="vspace">Login to stateu.org.
<img class="alignnone size-full wp-image-66" src="https://stateu.org/docs/wp-content/uploads/2018/03/login.png" alt="" width="477" height="320" /></li>
 	<li class="vspace">In the <strong>Search Box</strong> at the top of the page, search for “<abbr title="File Transfer Protocol">FTP</abbr>”, and click the <strong><abbr title="File Transfer Protocol">FTP</abbr> Accounts</strong> icon that appears.<img class="alignnone size-full wp-image-124" src="https://stateu.org/docs/wp-content/uploads/2018/03/2018-03-30-at-2.25-PM.png" alt="" width="812" height="339" /></li>
 	<li class="vspace">Every cPanel has an FTP account by default, and you can find those credentials by scrolling down on the FTP Accounts page. You also have the option to create a <em>new</em> <abbr title="File Transfer Protocol">FTP</abbr> account, which can be done by filling out the <strong>Add <abbr title="File Transfer Protocol">FTP</abbr> Account </strong>form with a username and password. Unless you change it, the new <abbr title="File Transfer Protocol">FTP</abbr> account will be limited to a directory with the same name as the account you're creating. You can change this to a different directory, if you want to grant this account access to a different location.  <strong>NOTE: Make sure you know/remember the password you enter.</strong> When you're done, click <strong>Create <abbr title="File Transfer Protocol">FTP</abbr> Account</strong>.
<img class="alignnone size-full wp-image-125" src="https://stateu.org/docs/wp-content/uploads/2018/03/2018-03-30-at-2.30-PM.png" alt="" width="808" height="573" /></li>
 	<li class="vspace">Once you've created the new account, you'll see it appear in the list at the bottom of the <abbr title="File Transfer Protocol">FTP</abbr> Accounts page. In addition to any accounts you've created, in the Special <abbr title="File Transfer Protocol">FTP</abbr> Accounts section, you'll see the default <abbr title="File Transfer Protocol">FTP</abbr> Account. You'll know this account because the username corresponds to your cPanel username. This <abbr title="File Transfer Protocol">FTP</abbr> account has full privileges to access all directories within your cPanel.</li>
 	<li class="vspace">For whichever account you need credentials for, click the <strong>Configure <abbr title="File Transfer Protocol">FTP</abbr> Client</strong> link. <img class="alignnone size-full wp-image-127" src="https://stateu.org/docs/wp-content/uploads/2018/03/2018-03-30-at-2.35-PM.png" alt="" width="1378" height="602" /></li>
 	<li class="vspace">Write down the username, server, and port information that appears. You will need to use this (or you will need to provide this to the person you are giving <abbr title="File Transfer Protocol">FTP</abbr> access) along with the password you created in Step 3 in order to configure your <abbr title="File Transfer Protocol">FTP</abbr> client.</li>
</ol>
PLEASE NOTE:

For cPanel's default FTP account, use the following settings:
<p style="padding-left: 30px;">-Connect via <strong>SFTP</strong> (more secure than FTP)
-Port: <strong>22</strong></p>
For an FTP account that you manually created (shown in Step 3 above), use the following settings:
<p style="padding-left: 30px;">-Connect via <strong>FTP</strong> (cPanel doesn't allow an SFTP connection for manual accounts)
-Port: <strong>21</strong></p>

</div>
<h2 id="configure-ftp-in-your-ftp-client" class="sectionedit4">Configure FTP in Your FTP Client</h2>
<div class="level2">

Below are links to tutorials for setting up both FileZilla and CyberDuck to connect to your <abbr title="File Transfer Protocol">FTP</abbr> account.
<ul>
 	<li class="level1">
<div class="li"><a class="urlextern" title="http://www.siteground.com/tutorials/filezilla/filezilla_management.htm" href="http://www.siteground.com/tutorials/filezilla/filezilla_management.htm" target="_blank" rel="nofollow noopener noreferrer">FileZilla Configuration Instructions</a></div></li>
 	<li class="level1">
<div class="li"><a class="urlextern" title="https://trac.cyberduck.io/wiki/help/en/howto/ftp" href="https://trac.cyberduck.io/wiki/help/en/howto/ftp" target="_blank" rel="nofollow noopener noreferrer">CyberDuck Configuration Instructions</a></div></li>
</ul>
For further assistance on FTP, <a href="https://community.reclaimhosting.com/t/ftp-file-transfer-protocol/304" target="_blank" rel="noopener noreferrer">read this guide</a>.

</div>