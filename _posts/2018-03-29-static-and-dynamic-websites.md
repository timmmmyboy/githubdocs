---
ID: 30
post_title: Static and Dynamic Websites
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=30
published: true
post_date: 2018-03-29 20:00:46
---
<div class="level2">
<h2 id="dynamic-websites" class="sectionedit3">Static Websites</h2>
In the early days of the Web, almost all Web sites were what is known as <code>'static sites.'</code> Content (text, images, video, audio, etc), was placed or embedded in a file in which HTML tags were used to format it. If you looked at the actual contents of the file, you might see something like this:

<img class="alignnone size-full wp-image-554" src="https://stateu.org/docs/wp-content/uploads/2018/03/8443925963_3511d91c7c_o.png" alt="" width="377" height="223" />

The content and the tags lived side-by-side. To edit the page, you'd open up the file (on your own computer) in a program capable of editing HTML files and make changes to either the content or the presentation. Every page had to be edited individually, even if the edits you were making were for common elements that appeared on many pages (like menu bars).

From a technical perspective, accessing a static Web site is fairly straightforward. When your computer is connected to the Internet, you can use a Web browser to access files on a Web server (as long as you know the address). The Web server delivers the contents of those files to your browser, and your browser displays them.

</div>
<h2 id="dynamic-websites" class="sectionedit3">Dynamic Websites</h2>
<div class="level2">

Over time, as the Web became more sophisticated, new systems emerged for creating and managing Web sites. These moved beyond the model of having content and <abbr title="HyperText Markup Language">HTML</abbr> tags live in a simple <abbr title="HyperText Markup Language">HTML</abbr> page which your browser accessed and displayed. Instead, these systems were Web applications – software that literally runs on the Web server and makes it possible to manage a Web site, often with very sophisticated features. One feature of these applications is that they separate content and presentation by storing most content (your text, images, etc) and data about the site (the title, options, etc). in a database.

On the Web server, the Web application installs files that are written in some kind of programming language. The server reads this code and obeys any requests in it to access data in the database (which lives on a separate server) and displays it according to the instructions in the code.

<img class="alignnone size-full wp-image-555" src="https://stateu.org/docs/wp-content/uploads/2018/03/8444050009_c541d8bba5_o.png" alt="" width="581" height="386" />

Essentially, the data for the site (living in a series of tables in a database on the database server) is entirely separate from the actual presentation of the site (living in the code of the programmed files on the Web server). Special software on both the Web server and the Database server enable the two to speak to each other and work together.

One of the benefits of using a Web application is that you usually don't need to touch (or even look at!) the code in order to make changes to your content. In addition, editing the site usually involves accessing some kind of control panel through your Web browser and filling out a form, instead of having to download and access files in software on your own computer.

</div>
<h2 id="dynamic-vs-static-content" class="sectionedit4">Dynamic vs Static Content</h2>
<div class="level2">

Sometimes when we talk about the difference between dynamic and static content we get bogged down in the idea of whether or not the content is “fresh” (dynamic, regularly updated) or “old” (static, never updated). How frequently you update your content has nothing to do with what kind of system you are using to manage your site. You can manage a static Web site (as described above) and update the content every day. You can also have a dynamic Web site (running something like WordPress) and never change the content after you create it.

Generally speaking, it <em>is</em> easier to regularly update content on a dynamic Web site because the Web application just makes it easier. Sometimes, even when you just want a very basic page or placeholder, it's easier to install a Web application (and only put up a single page) then to manually create an HTML page and upload it.

</div>
<h2 id="a-side-note-about-separating-content-from-presentationstyle-sheets" class="sectionedit5">A Side Note about Separating Content from Presentation: Style Sheets</h2>
<div class="level2">

Another aspect of separating content from presentation involves the use of <code>'Cascading Style Sheets'</code> (<abbr title="Cascading Style Sheets">CSS</abbr>). These are special files that live on your Web server and are linked to your Web pages. They contain information (written in a special markup language) about how to make elements on your site look. For example, they allow you to define in a single location what all Level 1 Headings look like on your site. They are an important aspect of understanding how to separate content from presentation, but they're not really an aspect of the difference between static and dynamic sites. Both static and dynamic sites can use style sheets.

</div>