---
ID: 212
post_title: Working with Omeka Classic
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=212
published: true
post_date: 2018-04-03 16:21:15
---
Here are a few tips and tricks that can help make sure you get the most out of the Omeka software.
<h2>ImageMagick</h2>
Omeka requires the ImageMagick library in order to resize and generate thumbnails for your images. State University provides ImageMagic for all accounts, but occasionally you will need to manually enter the server path to the utility. The setting for this is located under the <strong>Settings</strong> &gt; <strong>General</strong> tab and the path to ImageMagick is <strong>/usr/bin</strong>

<img src="https://stateu.org/docs/wp-content/uploads/2019/10/201910a5cd299aad7a8a3f74f461474ca93b27316ebcb4.png" alt="image" width="558" height="136" />
<h2>PHP-CLI</h2>
Some plugins including <a href="https://omeka.org/classic/plugins/CsvImport/" target="_blank" rel="noopener noreferrer"><strong>CSV Import</strong></a> and <a href="https://omeka.org/classic/plugins/Neatline/" target="_blank" rel="noopener noreferrer"><strong>Neatline</strong></a> may need to execute code using the command-line version of PHP. If your plugin requires this it can be enabled by editing the <strong>config.ini</strong> file in your File Manager under <strong>application&gt;config</strong>.

Navigate to the line that reads:
<pre>background.php.path = “”</pre>
Change it to the following:
<pre>background.php.path = "/usr/bin/php-cli"</pre>
&nbsp;