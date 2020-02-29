---
ID: 29
post_title: LAMP Environments
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=29
published: true
post_date: 2018-03-29 20:00:46
---
<div class="level1">

When you sign up for an account on Stateu.org, you get a personal space our web host. There are a few things you need to know about the Web host that will make it easier to understand what you can do with your new space.

</div>
<h2 id="the-web-server" class="sectionedit2">The Web Server</h2>
<div class="level2">

The Web server is the main computer that is associated with the stateu.org hosting account. It is literally a computer that has special software on it that allows it to be accessible via the Web. The files that run your applications, images, video, or any other files you upload into your Web space are stored on this server.

(For comparison's sake, your desktop or laptop computer, by default, doesn't allow this; I can't access files on your computer through a Web browser by default. You <em>can</em> actually install Web server software on your own computer, however, essentially making your files accessible over the Web.)

In order to run properly, a Web server has to have an operating system installed <em>and</em> some kind of Web server software. Our State University hosting environment runs the <code>LINUX</code> operating system and an <code>APACHE</code> Web server.

</div>
<h2 id="the-database-server" class="sectionedit3">The Database Server</h2>
<div class="level2">

In addition to the Web server, there is also an associated database server. This is another computer, but it is configured with software that allows it to host databases. It is also connected to your Web server so that your applications (hosted on the Web server) can retrieve data (from databases hosted on the database server).

Databases come in many varieties. The kind of database you can use for a Web application depends on the kind of software that's installed on the database server. Our State University hosting environment runs <code>MYSQL</code> databases.

</div>
<h2 id="the-programming-language" class="sectionedit4">The Programming Language</h2>
<div class="level2">

When you install open-source software on your Web account, it's going to be written in a programming language. Our State University hosting environment has software installed on it that allows it to understand different programming languages. If you install software that's written in a language that your Web server doesn't read, it won't work.

The StateU hosting environment can currently interpret <code>PHP</code>, <code>PERL</code>, and <code>PYTHON</code>.

</div>
<h2 id="add-it-togetherlamp" class="sectionedit5">Add it Together: LAMP</h2>
<div class="level2">

If you take a look at all the descriptions above, you can determine that we are running what is known as a LAMP server for stateu.org:
<ul>
 	<li class="level1">
<div class="li"><strong>L</strong>inux (operating system)</div></li>
 	<li class="level1">
<div class="li"><strong>A</strong>pache (Web server)</div></li>
 	<li class="level1">
<div class="li"><strong>M</strong>ySQL (database server)</div></li>
 	<li class="level1">
<div class="li"><strong>P</strong>HP/PERL/PYTHON (programming language)</div></li>
</ul>
Applications that are written for LAMP environments will, presumably, run on the server. <em>However</em>, some applications do require additional extensions or libraries that aren't included in a LAMP environment by default. The applications you can install via Installatron (in cPanel) should work just fine.

LAMP environments are unique because all components are open-source, meaning Linux, Apache, MySQL, PHP, PERL, and PYTHON are open for anyone to use for free. Anyone can also modify them and redistribute them. As a result, there are lots of online resources for using these systems that have been built by their communities of users. But, also as a result, since you're not paying for these systems, you can't just call up a company and ask them to fix a problem.

</div>