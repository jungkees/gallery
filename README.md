Gallery API demo
=======
Overview
--------
This repo contains the source code for a demo to discuss on the Gallery API proposed at W3C DAP WG.
Gallery API works based on Web Intets pick request and the corresponding response in callback.

The demo includes two scenarios: [1] Pick images by URL and [2] Pick images by Content 

[1] retrieves only image URLs with metadata and display images using
<pre>
 &lt;img src=the image url /&gt;
</pre>

[2] receives actual image contents with metadata and display images using
<pre>
 &lt;img src="data: image/jpeg, " + the image content +'"' /&gt;
</pre>

* Environment:
Chrome 19.0.1084.52 stable or higher (for Web Intents support)

How to run
----------

1. download the manifest files for [1] and [2] from:

  (a) https://github.com/jungkees/gallery/blob/master/manifest/url/manifest.json
      https://github.com/jungkees/gallery/blob/master/manifest/url/G.png
     
  (b) https://github.com/jungkees/gallery/blob/master/manifest/content/manifest.json
      https://github.com/jungkees/gallery/blob/master/manifest/content/G.png
     
2. Save (a) at your local storage

   1) manifest.json and G.png should be stored at the same folder.
   
   Do the same for (b) (at different folder)
   
3. Register Intents (a) and (b) by: 

   1) Load "chrome://chrome/extensions" page in Chrome
   
   2) Click "Load unpacked extension..." button
   
   3) Go to the folder having (a)
   
   4) Click "Open"
   
   Do the same for (b)
   
4. go to:
  http://jungkees.github.com/gallery/
5. Click "Pick" button and select the corresponding intent request from picker registered at 3.

Server
------
The demo server has been implemented as node.js app. The service runs at Nodester hosting server.

