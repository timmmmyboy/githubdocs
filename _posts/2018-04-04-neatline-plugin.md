---
ID: 286
post_title: Neatline Plugin
author: admin
post_excerpt: ""
layout: post
permalink: https://wpdocs.timowens.io/?p=286
published: true
post_date: 2018-04-04 16:54:14
---
<h3>Building an interactive map using Omeka’s Neatline plugin</h3>
Neatline is a plugin for Omeka that allows for the creation of interactive maps and timelines. Neatline allows the user to plot points on geospatial layers that, when clicked, reveal text and media. Users may create records from scratch and add them to their Neatline exhibits, or import existing items from Omeka. See <a href="http://neatline.org/" target="_blank" rel="noopener noreferrer">Neatline.org</a> for demos of this tool in action and more documentation.

Before using this tool, you’ll need to <strong>install the Neatline plugin to Omeka</strong>. If you’ve already installed the Escher plugin, you can use it to install Neatline. If not, follow the instructions on <a href="https://www.stateu.org/docs/#installing-plugins" target="_blank" rel="noopener noreferrer">the “Installing Plugins” section of this support page</a>.
<h3>Vocabulary</h3>
<strong>Item</strong>: Omeka’s basic building block, containing text, media, and/or metadata.
<strong>Collection</strong>: A group of items, typically sharing a common theme.
<strong>Record</strong>: Neatline’s version of items. Can be created on their own, or imported from an existing item in Omeka.
<strong>Exhibit</strong>: A Neatline map or timeline; contains your records.
<strong>Widget</strong>: An add-on tool for Neatline, such as Waypoints.
<strong>Spatial layer</strong>: A navigable map that Neatline can use, typically pulled from Google Maps. The various options Neatline offers have different aesthetics.
<h3>Setting up (first time only)</h3>
1. Install the Neatline plugin (see above). Install any additional supporting plugins you’d like, such as Neatline Waypoints.

2. Go to your Plugins page in Omeka. Then, click “Configure” to the right of Neatline. On the configuration page, click the link to <a href="http://developers.google.com/maps/web" target="_blank" rel="noopener noreferrer">developers.google.com/maps/web</a>. If possible, open this link in a new tab, since you’ll soon need to return to the configuration page.

<img class="alignnone size-full wp-image-288" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.12-PM.png" alt="" width="1239" height="723" />

<img class="alignnone size-full wp-image-289" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.19-PM.png" alt="" width="1144" height="780" />

<img class="alignnone size-full wp-image-290" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.20-PM.png" alt="" width="1243" height="720" />

3. On the Google page that opens, click the “GET A KEY” button at top right. Follow the prompts in the pop-up window to create a new project, named whatever you’d like (this title won’t matter for your Neatline projects). When you’re given a long string of characters, copy it. This is your Google Maps API Key. You’ll only need it once.

<img class="alignnone size-full wp-image-398" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191004-API-step2-getkey.jpg" alt="" width="1440" height="850" />

4. Return to the Neatline configuration page from step 2. Paste your API Key into the text box. Then click the green “Save Changes” button. Neatline is now connected to Google Maps.

<img class="alignnone size-full wp-image-291" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.21-PM.png" alt="" width="1258" height="729" />

5. Click Settings at top right of your Omeka dashboard. In the text box to the right of “ImageMagick Directory Path,” enter this exact text without the quotation marks: “/usr/bin”. Then click the green Save Changes button at top right. This will allow Omeka to handle your images properly.

<img class="alignnone size-full wp-image-292" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.22-PM.png" alt="" width="1079" height="780" />

Neatline is now ready to go!
<h3>Laying the foundation</h3>
<strong>1. Optional: create one or more collections.</strong> This is an organizational tool: by creating collections now, you’ll be able to sort your items or bulk import them to Neatline more easily later. To create a collection, click “Collections” on your lefthand Omeka dashboard menu. Then, click the green Add a Collection button. On the Add a Collection page, give your collection a Title (you can leave all other boxes blank). If you want to add formatting to your text such as bolding or italics, check the box next to “Use HTML,” and more editing options will appear.

When you’re done, check the box next to “Public” and then click the green Add Collection button.

<strong>NOTE</strong>: You’ll see many fields when creating collections or items, but there’s no need to panic: almost all are optional and exist for archival purposes. Only fields with a * after them are required.

<img class="alignnone size-full wp-image-294" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.24-PM.png" alt="" width="1159" height="780" />

<strong>2. Begin creating items.</strong> Omeka is a tool for curating artifacts. In this step, you’ll begin this curation by creating items. To create an item, click “Items” on your lefthand Omeka dashboard menu. Then, click the green Add an Item button. On the Add an Item page, give your item a Title and a Description (you can leave all other boxes blank). This is the text that will ultimately appear to viewers of this record on your Neatline map. If you want to add formatting to your text such as bolding or italics, check the box next to “Use HTML,” and more editing options will appear.

Check the box next to “Public.” If you wish to add this item to a collection, select it from the dropdown menu under “Collection.”

If you wish to add images to your item, click the “Files” tab, then click “Choose File.” Follow the prompts to upload an image. To upload more images, click the green Add Another File button. These images will be displayed alongside your text when a viewer clicks the relevant point on your map.

If you wish to add tags to your item, click the “Tags” tab, then enter all desired tags in the text box, separated by commas. Remember to click Add Tag afterward.

<img class="alignnone size-full wp-image-296" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.26-PM.png" alt="" width="1148" height="783" />

<img class="alignnone size-full wp-image-297" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.27-PM.png" alt="" width="1267" height="730" />

<img class="alignnone size-full wp-image-298" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.29-PM.png" alt="" width="1278" height="734" />

When you’re done adding text, files, and tags, click the green Add Item (or Save Changes if you’re editing) button.

You can always find your list of items, with the option to edit each one, by clicking Items on your Omeka dashboard. From the Items page, you can also use the blue Search Items button to filter items by user or tag.

<img class="alignnone size-full wp-image-300" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.30-PM.png" alt="" width="1203" height="781" />

Clicking “Tags” on the Omeka dashboard will bring you to a list of all your tags. Click a tag’s name to edit it, or click the number to its left to view all items with that tag.

<img class="alignnone size-full wp-image-301" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.33-PM.png" alt="" width="1276" height="726" />
<h3>Managing Neatline exhibits and using the editor</h3>
<strong>1. Create an exhibit.</strong> Your Neatline map will be known as an exhibit. It’s now time to create this map. Click Neatline on the lefthand dashboard menu, which brings you to the Browse Exhibits page. Then click the green Create an Exhibit button.

<img class="alignnone size-full wp-image-303" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/10-neatline-exhibits.jpg" alt="" width="1246" height="645" />

On the Create an Exhibit page: give your exhibit a Title, Narrative (optional but recommended), and Widgets (if you’d like to use Waypoints or another add-on you’ve previously installed). The Narrative is the exhibit’s primary textual description, and it will appear alongside your map.

<img class="alignnone size-full wp-image-304" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/11-create-exhibit-1.jpg" alt="" width="1254" height="886" />

Scroll down and select a Default Spatial Layer from the drop-down menu. The Default Spatial Layer is the default map style your exhibit will display. You can edit this any time, so try out a few and see which aesthetic you like best. You can also optionally use the Embed Spatial Layers field to allow your viewers to toggle between various map styles.

The only other setting you need to change here (eventually) is Public: when you check this box, your exhibit will be live. When you’re done, click the green Save Exhibit button at the bottom of the form.

<img class="alignnone size-full wp-image-305" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/12-create-exhibit-2.jpg" alt="" width="1260" height="908" />

<strong>2. Access the Neatline editor.</strong> Return to the Browse Exhibits page from step 1. To access the editor, click your exhibit’s title. Clicking Public View or Fullscreen View will let you preview how your exhibit will look to visitors.

<img class="alignnone size-full wp-image-306" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/13-access-editor.jpg" alt="" width="1264" height="689" />

Here is what the editor looks like. Notice the Records, Styles, and Plugins tabs, and the list of records below the blue New Record button (there won’t be any records until you add some):

<img class="alignnone size-full wp-image-399" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191014-editor.jpg" alt="" width="1914" height="951" />

<strong>3. Set the default focus.</strong> This is the latitude/longitude and zoom that viewers will see when they first open your map (they’ll then be able to move it however they’d like). In the editor, click the Styles tab. Click and drag on your map to move it around, and use the + and – symbols at top left to zoom in and out. When you’re satisfied with the current view of the map, click the Use Current Viewport as Default button. This will automatically fill-in coordinates and the depth of zoom. You can also manually add these. When you’re done, click the blue Save button.

<img class="alignnone size-full wp-image-400" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191015-default-focus.jpg" alt="" width="1916" height="948" />

<strong>4. Import items into your exhibit</strong>, which then become records. First, click the Records tab in the editor. Then, click the large blue New Record button.

<img class="alignnone size-full wp-image-401" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191016-new-record.jpg" alt="" width="1917" height="948" />

New tabs will appear. Click the Item tab. You’ll see a drop-down menu called “Search Omeka items.” This will list all the Omeka items you’ve previously created. Find the item you wish to add to the map and select it. The item’s content appears below the drop-down menu. If it looks correct, click the blue Save button. If not, click “View the item in Omeka,” edit the item, and try again.

<strong>NOTE</strong>: If you edit an item in Omeka that you’ve already imported into your Neatline exhibit, its record in the exhibit will be automatically updated.

<strong>NOTE #2</strong>: You can also create records from scratch using the New Record button and the Text tab (without making an Omeka item first). However, this isn’t recommended if you wish to include images or other media in your record, since that media would require additional HTML formatting.

<img class="alignnone size-full wp-image-402" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191017-link-to-omeka.jpg" alt="" width="1916" height="946" />

<strong>5. Pin your records to the map.</strong> You can access any of your records from the list of records on the editor’s main page (see the screenshot in step 2 of this section, looking under the New Record button). Once you’re in a record, you can place it on the map. If you’ve just created a record using the Item tab from the previous step, then you’re already in that record.

Once in the record, click the Map tab. You can draw many different shapes here (and feel free to experiment!), but for our purposes, we’ll look at two buttons: “Navigate” and “Draw Point.”

When “Navigate” is selected, you can move your map around without adding anything. When “Draw Point” is selected, you can click on the map to place a blue pin. When a viewer clicks this pin, she’ll see the record associated with it. When you’re done, click Save.

For example: I have a record containing text and images about Shakespeare’s first performance of <em>Henry V</em> in London. I can go into my Henry V record and use “Draw Point” to place a pin on London. Now, the viewer can click the blue dot on London to bring up this record.

<img class="alignnone size-full wp-image-403" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191018-draw-point.jpg" alt="" width="1917" height="952" />

Optionally, you can use the Style tab in a record (to the right of the Map tab) to change the appearance of points and shapes for that record.

You can add as many interactive points or shapes as you’d like.

<strong>6. Add widgets to your record (optional). </strong>If you’re using the Waypoints widget, select it by clicking in the Widgets field. See the next step for more information about Waypoints.

When you’re done, click Save. Then, you can exit out of the record and back to the editor’s main page by clicking the X above the Style tab. You can return to Omeka by clicking “Return to Omeka.”

<strong>7. Adding Waypoints: a table of contents for your map.</strong> The following guide from Neatline.org explains how to add a list of clickable records to your map, so viewers can jump from point to point without searching the map for them:
<a href="http://docs.neatline.org/working-with-the-waypoints-plugin.html" target="_blank" rel="noopener noreferrer">http://docs.neatline.org/working-with-the-waypoints-plugin.html</a>

<img class="alignnone size-full wp-image-405" src="https://wpdocs.timowens.io/wp-content/uploads/2019/10/20191020-waypoints.jpg" alt="" width="1910" height="950" />
<h3>Linking your maps to your Omeka home page</h3>
<strong>1. Choose what links you’d like to display on your home page’s navigation menu.</strong> This menu may appear in a slightly different place on your homepage depending on your theme. Here’s what it looks like in one of Omeka’s built-in themes (“Thanks, Roy”):

<img class="alignnone size-full wp-image-308" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/21-frontpage-default.jpg" alt="" width="1695" height="713" />

<strong>To edit this menu</strong>: from your Omeka dashboard, click Appearance in the black bar at the top of the screen. Then click the Navigation tab.

<img class="alignnone size-full wp-image-309" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/2018-04-04-at-12.42-PM.png" alt="" width="1151" height="779" />

This takes you to a checklist of links. Each checked link will appear on your home page’s menu. To edit a link’s label (name) or URL, click the small black arrow to its right.

<strong>To add a new link</strong>: fill in the Label and URL fields at the bottom of this page, and then click Add Link. You can reorder the menu by clicking and dragging the links. When you’re done, click the green Save Changes button.

<img class="alignnone size-full wp-image-310" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/23-appearance-navigation2.jpg" alt="" width="1290" height="762" />

By default, there will be a link called “Neatline” which takes your viewer to a list of your Neatline exhibits. This is called the Browse Exhibits page, and looks like this:

<img class="alignnone size-full wp-image-311" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/24-frontpage-browse-exhibits.jpg" alt="" width="1898" height="475" />

If you’d rather have links on your menu to one or more specific exhibits, first pull up that exhibit’s public or full-screen view (see the screenshot for step 2 under <em>Managing Neatline exhibits and using the editor</em> above). Copy the URL from the address bar at the top of your browser. Paste it into the URL field on Appearance &gt; Navigation, give it a label, click Add Link, and then Save Changes.

<strong>2. OR, choose a different default home page.</strong>

<em>To use a list of your Neatline exhibits as your home page</em>:
On Appearance &gt; Navigation, click on the drop-down menu under “Select a Homepage” (to the right of the link checklist). Select “Neatline” (or whatever you’ve renamed it). Click Save Changes to finish.

<img class="alignnone size-full wp-image-312" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/25-appearance-navigation3.jpg" alt="" width="1294" height="776" />

<em>To use a specific exhibit as your home page (taking your viewer directly to the map)</em>:
On Appearance &gt; Navigation, add a link to the public or fullscreen view of the map you wish to be the homepage (see the previous step). Then, click on the drop-down menu under “Select a Homepage” (to the right of the link checklist). Select the link you’ve just added. Click Save Changes to finish.

<img class="alignnone size-full wp-image-313" src="https://wpdocs.timowens.io/wp-content/uploads/2020/02/26-appearance-navigation4.jpg" alt="" width="1270" height="819" />

Now you can share your Omeka site’s address with whomever you’d like, and they’ll be able to explore your interactive map!