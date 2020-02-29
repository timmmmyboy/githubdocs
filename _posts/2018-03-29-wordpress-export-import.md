---
ID: 21
post_title: WordPress Export/Import
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=21
published: true
post_date: 2018-03-29 20:00:46
---
<div class="doc-sec-content">

If you are using your WordPress, you can also get an export of your posts, pages, comments, custom fields, categories, and tags.

The Wordpress export is great for grabbing the content of your WordPress site so that you can import it into another Wordpress host, such as Wordpress.com or Wordpress.org.
<blockquote>Note: Exports do not include plug-ins, or other site customizations.</blockquote>
<h2>Exporting</h2>
<ol>
 	<li class="vspace">From the<strong> Dashboard </strong>navigate to <em>Tools&gt;Export</em><strong><strong>
</strong></strong>The screenshot below shows how to export all of your posts, pages, comments, custom fields, terms, navigation menus, and custom posts. However, you can also export just certain posts, pages, or media.<strong> <img class="shadow alignnone wp-image-545 size-full" src="https://stateu.org/docs/wp-content/uploads/2019/10/201910wordpress-export.png" alt="The export page within WordPress" width="1018" height="829" />
</strong></li>
</ol>
This export process generates an XML file of your blog’s content. WordPress calls this an  eXtended RSS or WXR file.

<strong>Note:</strong> This will ONLY export your <strong>posts, pages, comments, categories, and tags</strong>; uploads and images <em>may</em> need to be manually transferred to the new blog. If possible, do not delete your blog until after media files have successfully been imported into the new blog.
<h2>Importing</h2>
Once you have exported your posts, pages, etc., you can import them into your new WordPress site.
<ol>
 	<li class="vspace">Login to your new WordPress.com or self-hosted WordPress site and go to the Dashboard.  From there navigate to <em>Tools&gt;Import</em> and click on the link to "<em>Run Importer</em>"<strong>
<img class="shadow alignnone wp-image-546 size-full" src="https://stateu.org/docs/wp-content/uploads/2019/10/201910worpress_run_importer.gif" alt="Screenshot showing where to find the Wordpress Importer" width="1146" height="857" /></strong></li>
 	<li class="vspace"> Next you will see a screen that prompts you to upload the WXR (.xml) file you generated through the export process. Browse to your exported Wordpress archive and then click the "<em>Upload file and import</em>" button.
<img class="shadow alignnone wp-image-544 size-full" src="https://stateu.org/docs/wp-content/uploads/2019/10/201910worpress_import1.gif" alt="Upload file and import" width="1018" height="831" /></li>
 	<li class="vspace">Choose and upload your file.  You will then be prompted to assign an author to the posts that you are importing.  You can use this function to assign one author to all posts, or you can manually set the author for each post in the posts menu. Unless you have a space limit, you will also want to select the option to "download and import file attachments" before clicking the "<em>Submit</em>" button.
<img class="shadow alignnone wp-image-543 size-full" src="https://stateu.org/docs/wp-content/uploads/2019/10/201910worpress_import2.gif" alt="Select desired import options and click the " width="1018" height="832" /></li>
 	<li class="vspace">When your import is complete, you will see a confirmation screen.
<img class="shadow alignnone wp-image-542 size-full" src="https://stateu.org/docs/wp-content/uploads/2019/10/201910worpress_import3.gif" alt="Confirmation screen" width="1018" height="830" /></li>
</ol>
Your exported content is now added to your site. If you had posts on your site prior to importing, those posts are still available.

Because the export did not include themes or plug-ins, you will need to reinstall those separately from the export/import process.

</div>