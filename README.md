hoodie-pocket-UIKit
===================

**NOTE: the functionality described here is for version 2.0.0 or higher (should be included with any hoodie-server with a version _above_ 0.9.26).**

![Screenshot of a plugin styled by the UIKit](pocket_uikit_screenshot.png)

Pocket UIKit is a collection of CSS styles and JS libraries for easier and faster building of Pocket components for Hoodie Plugins. It includes neat form styles, better select drop-downs with autocomplete, drag-n-drop file upload fields, better checkboxes etc. 
We encourage the use of this kit when building your own plugins so 

1. you don't have to worry about styling, and 
1. all plugins have a consistent look in their admin panels

It includes a static test page of all available elements that you can copy and paste for use in your Pocket components, this is at `http://yourhoodieendpoint/_api/_plugins/_assets/index.html`.

## Including the UIKit in your plugin's Pocket component

Put this in the `<head>`:`<link rel="stylesheet" href="/_api/_plugins/_assets/styles/pocket-uikit.css">
`

And this before the closing `</body>` tag: `<script src="/_api/_plugins/_assets/scripts/pocket-uikit.js"></script>
`

You'll get basic styles and behaviour for a bunch of UI elements, including nicer checkboxes/radio buttons and better select dropdowns. 

You can also have drag n' drop file uploads, please consultthe aforementioned `index.html` as well as `/_api/_plugins/_assets/scripts/main.js` for an example of the frontend aspect of this.

In the future, these will be part of a `my-first-plugin`-repo you can use as a base for your own plugins. Also, there will be a docs page with copy-and-pastable examples and clearer usage explanations.

To explore the UIKit further, browse through `http://yourhoodieendpoint/_api/_plugins/_assets/` (final slash matters, sorry). This base path will show you an index of all available files. 

## Development

Install dependencies and run the preview app on a local webserver with livereload.

```bash
npm install -g grunt-cli bower
npm install
bower install
grunt server
```
