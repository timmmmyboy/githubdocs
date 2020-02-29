---
ID: 318
post_title: Managing Backups
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=318
published: true
post_date: 2018-04-04 19:22:29
---
Any application that you install in State University using the cPanel/Installatron is set to automatically create a backup of the whole app every time the software updates. The backups expire after 14 days, but they can quickly eat up quota space in that time, especially since some apps (such as WordPress) update automatically. Follow the steps in each section below to take more control over the space that backups use in your account.
<h4>1. Turn off the automatic Installatron backup</h4>
<ul>
 	<li>Go to your cPanel</li>
 	<li>Go to <strong>Applications</strong> &gt; <strong>WordPress</strong> &gt; <strong>My Applications</strong>.</li>
 	<li>From there, select the wrench next to your site’s name.</li>
 	<li>Scroll down to Automatic Update Backup and set that to <strong>Do not create a backup</strong></li>
</ul>
<img class="alignnone wp-image-123 size-full" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_AutomaticUpdateBackup.png" sizes="(max-width: 1562px) 100vw, 1562px" srcset="https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_AutomaticUpdateBackup.png 1562w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_AutomaticUpdateBackup-300x144-1.png 300w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_AutomaticUpdateBackup-768x369.png 768w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_AutomaticUpdateBackup-1024x492-1.png 1024w" alt="Application Backups screen with an arrow pointing to &quot;Do not create a backup&quot; under &quot;Automatic Update Backup&quot;" width="1562" height="750" />
<h4>2. View restore points in R1Soft Backups App</h4>
The R1Soft Restore Backups app can be found in the “Files” section of your cPanel dashboard.

<img class="alignnone size-full wp-image-298" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_R1SoftLocation.png" sizes="(max-width: 1363px) 100vw, 1363px" srcset="https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_R1SoftLocation.png 1363w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_R1SoftLocation-300x42-1.png 300w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_R1SoftLocation-768x106-1.png 768w, https://wpdocs.timowens.io/wp-content/uploads/2019/10/201910Build_R1SoftLocation-1024x142.png 1024w" alt="Files section of cPanel with R1Soft Restore Backups circled" width="1363" height="189" />

This app should already be active so there are no additional steps you need to take to set it up. R1Soft automatically creates an off-site backup of your files and databases nightly. You can open the app from your cPanel to verify that there are restore points listed. More information about how this app works can be found in this documentation from our hosting provider, Reclaim Hosting, under the “Automated Offsite Backup” heading: <a href="https://reclaimhosting.com/backups-done-right/" target="_blank" rel="noreferrer noopener">https://reclaimhosting.com/backups-done-right/</a>.
<h4>3. Create a manual Installatron backup before major changes</h4>
While R1Soft creates daily backups of all of your content, it’s best practice to have a backup of your application from right before you start tinkering, just in case anything goes wrong. That way you won’t lose any content that’s been added or changed since the latest daily backup. As a bonus, backups created through the Installatron are easy to restore with a single click. These manual backups can even be sent to an offsite location like Dropbox to save space.

To create a manual backup:
<ul>
 	<li>From your cPanel, click <strong>My Apps</strong> in the <strong>Applications</strong> section.</li>
 	<li>Click the checkbox to the far right of the application name (labeled 1 in the screenshot below).</li>
 	<li>Click “Backup” below the bottom of the application list (labeled 2 in the screenshot below).</li>
 	<li>On the next screen, enter a descriptive label and click Backup again. The backup will run with a status bar.</li>
</ul>
<img class="alignnone wp-image-319 size-full" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-3.21-PM.png" alt="" width="1403" height="416" />​