---
title: Javascript trick to edit the page displayed

date: 2007-01-21
url: /2007/01/21/javascript-trick-to-edit-the-page-displayed/
categories:
  - Fun
  - Tips and Tricks

---
Do you want to quickly edit the text of any webpage that you are browsing? Maybe you wanted to see how the site looks if you change some words. Here is a neat Javascript trick that you can use to edit the text part of the web page.

Do note that you can&#8217;t save the changed text onto the server or is this any means to hack a web server. If you refresh the page, all the changes you made will disappear. You can however save the resulting HTML if you goto `File -> Save as`.

Step 1: Drag this <a href="javascript:if (document.designMode=='off') { document.body.contentEditable='true'; document.designMode='on';} else { document.body.contentEditable='false'; document.designMode='off';} void 0">Edit/View</a> bookmarklet into your bookmarks toolbar. 

Step 2: Goto the web page which you want to edit and click on the bookmarklet &#8211; you will be put into the edit mode. Click the bookmarklet again and you will be put into the normal view mode.

Step 3: ?????

Step 4: Profit.

For those of you who like to know what it does beneath the scenes, it just sets two properties of the document to make it editable.

`javascript:document.body.contentEditable='true'; document.designMode='on'; void 0`
