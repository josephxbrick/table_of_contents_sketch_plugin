# Table of contents: a Sketch plugin

Note: this plugin requires Sketch 53.1 or above.

This sketch plugin creates a table of contents for artboards on the current page. If your document has sections, it will organize the table of contents into sections. Here is an example of what that looks like:

<img src="/readme_images/toc_image.png" width="900">

The TOC will live in a group on whichever page you wish. It will arrange itself into however many columns it needs depending on the height the group. (The plug-in will prompt you for the pixel spacing between columns.) Once the TOC created, you can size this group, and the TOC will rearrange itself as you size it.

You can completely define the look of it, as the plug-in uses symbols to create the TOC items, which you can customize to your liking.

## Setting up your Sketch file

For this plug-in to work, you'll need to set up your document in a specific way. Check out the sample.sketch file in this repository.

These are the elements that you will need in your document:

The group that the TOC will live in needs to be called `<tocGroup>` This group must contain a rectangle named `<tocGroupRect>`:

<img src="/readme_images/toc_group.png" width="218">



* Each artboard that you want listed in the TOC will need two symbol instances: one containing the name of the page or section, and another containing the page number. Note that a single symbol can contain both, as the plug-in only cares what the text override is named. However, the page number and page name can't be in a nested symbol.
* The text override name for the page title needs to be named 



