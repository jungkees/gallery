Gallery API demo
=======

This repo contains the source code for a demo to discuss on the Gallery API proposed at W3C DAP WG.
Gallery API works based on Web Intets pick request and the corresponding response in callback.

The demo includes two scenarios: [1] Pick images by URL and [2] Pick images by Content 

Environment:
Chrome 19.0.1084.52 stable or higher (for Web Intents support)

To try the demo, 

1. download the manifest files for [1] and [2] from:

  (a) https://github.com/jungkees/gallery/blob/master/manifest/url/manifest.json
      https://github.com/jungkees/gallery/blob/master/manifest/url/G.png
     
  (b) https://github.com/jungkees/gallery/blob/master/manifest/content/manifest.json
      https://github.com/jungkees/gallery/blob/master/manifest/content/G.png
     
2. Save (a) and (b) at your local storage
3. Register Intents (a) and (b)
  full instruction at)
4. go to:
  http://jungkees.github.com/gallery/
5. Click "Pick" button and select the corresponding intent request from picker.

The demo server reads image files from the storage and sends runs at gallery.nodester.com

