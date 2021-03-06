---
ID: 170
post_title: Publishing Content
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=170
published: true
post_date: 2018-04-02 15:15:37
---
<div class="level1">

The primary activity that you're likely to be doing on your WordPress site is publishing content. The content could be the text you write, pictures you take, videos or audios (which may be hosted on another site), or other media that you've found elsewhere on the Web. WordPress makes it very easy to publish media content of all types, whether hosted on your actual Web server or elsewhere.

</div>
<h2 id="posts-vs-pages" class="sectionedit11">Posts vs. Pages</h2>
<div class="level2">

Out of the box, WordPress provides two primary content types for you two work with: posts and pages. If you read blogs or have ever written for a blog before, the concept of a post is probably a bit familiar. <strong>Posts</strong> often are content that appear on your blog in some kind of scheduled way. They usually are presented on your site in reverse-chronological order. Posts might be what you use to share your regular thoughts, reflections, or ideas about a topic. Posts make up a kind of “river” of content that you're producing as part of your blogging activity.

<strong>Pages</strong> usually correspond to our more traditional concept of what makes up a Web site. Pages are presented outside of the “river” of content that are posts. They are more likely to stand alone and be organized according to a traditional hierarchy. Pages might be content that is less frequently updated or changed.

If you were using WordPress to build a business Web site with a lot of information content, you would probably use Pages. If you added a feature to that site where you started to advertise special events or news, you would probably use Posts.

<strong>A few other things to know about Pages vs Posts:</strong>
<ul>
 	<li class="level1">
<div class="li">If you want your content to be accessible to your users via RSS/syndication, you'll need to use Posts. By default, Pages do not appear in a site's RSS feed.</div></li>
 	<li class="level1">
<div class="li">Categories and Tags (which are used in WordPress to help you organize your content) are ONLY available on Posts. Page organization is done by customizing your site's menus.</div></li>
 	<li class="level1">
<div class="li">Okay, this get's a little tricky: WordPress, by default, also creates “Category Pages” and “Tag Pages” that display all the Posts in a category or tag. These are NOT related to the regular Page type.</div></li>
</ul>
</div>
<h2 id="media" class="sectionedit12">Media</h2>
<div class="level2">

Upon occasion, you may want to include media (images, audio, video) in your site's posts and pages. There are generally two approaches to handling media in WordPress:

<strong>Uploading</strong>: You can upload the files to your site's Media Gallery and then link to them in your posts/pages. This works very well for images, and when you take this approach for images you have the added benefit of being able to make use of WordPress' built-in (albeit rudimentary) editing tools. Also, when you upload images to WordPress, it automatically creates different sizes that you can use, as needed. This approach works less well for audio and video. In order to have your media files actually show up in a “player” (with controls for stopping, pausing, etc.) you'll need to install a plugin. Otherwise, you'll only be able to include links to the files. How people view/listen to them will depend a bit on the setup on their own computer and in their own browser. They may, for example, have to download the media file and then open it in another program on their computer.

<strong>Embedding</strong>: You can embed media from other sites easily in WordPress. Embedding an image just means providing a <abbr title="Uniform Resource Locator">URL</abbr> to its location elsewhere on the Web. Instead of uploading it to the server, WordPress grabs that image from the external source and displays it on your post/page. However, with this approach, you lose your editing capabilities as well as the resizing feature. Embedding audio and video from external sources becomes easier with every version of WordPress it seems. These days, you can embed video and audio from many external services (YouTube, Vimeo, SoundCloud, complete list here) by simply placing the full <abbr title="Uniform Resource Locator">URL</abbr> of the audio/video location on its own line in your post/page. There is <a class="urlextern" title="http://codex.wordpress.org/Embeds#Okay.2C_So_What_Sites_Can_I_Embed_From.3F" href="http://codex.wordpress.org/Embeds#Okay.2C_So_What_Sites_Can_I_Embed_From.3F" target="_blank" rel="nofollow noopener noreferrer">a complete list of supported external services</a>, and you can learn <a class="urlextern" title="http://codex.wordpress.org/Embeds" href="http://codex.wordpress.org/Embeds" target="_blank" rel="nofollow noopener noreferrer">more about embedding from external sources at the WordPress site</a>. Our general advice is to use externally hosted media whenever it makes sense and works. This is <em>usually</em> the case when you need to use audio or video; without plugins, well-presented audio and video in WordPress is tricky. For images, if you need to do basic editing and/or require different sizes of images, upload them to your site. Otherwise, consider referencing them from another location (your Flickr account, for example).

</div>
<h2 id="post-formats" class="sectionedit13">Post Formats</h2>
<div class="level2">

Recent versions of WordPress have built out a new “post format” feature which, if you are using a theme with the feature enabled, will style post formats differently depending on what they are. The formats that are built-in to WordPress (and are available for theme developers to use) are the following:
<ul>
 	<li class="level1">
<div class="li">aside - Similar to a Facebook note update.</div></li>
 	<li class="level1">
<div class="li">gallery - A gallery of images.</div></li>
 	<li class="level1">
<div class="li">link - A link to another site.</div></li>
 	<li class="level1">
<div class="li">image - A single image.</div></li>
 	<li class="level1">
<div class="li">quote - A quotation.</div></li>
 	<li class="level1">
<div class="li">status - A short status update, similar to a Twitter status update.</div></li>
 	<li class="level1">
<div class="li">video - A single video.</div></li>
 	<li class="level1">
<div class="li">audio - An audio file.</div></li>
 	<li class="level1">
<div class="li">chat - A chat transcript.</div></li>
</ul>
Those of you familiar with <a class="urlextern" title="http://tumblr.com/" href="http://tumblr.com/" target="_blank" rel="nofollow noopener noreferrer">Tumblr</a> may recognize this approach to post formats.

For the most part, post formats are designed as a way to <strong>style</strong> a site (and customize styling depending on the kind of content that is being displayed). They have no special functionality, and their use depends entirely upon the theme you are using. Many older themes, for example, do not recognize post formats.

</div>