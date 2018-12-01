---
title: Firefox unresponsive scripts warning – fix

date: 2006-02-05
url: /2006/02/05/firefox-unresponsive-scripts-warning-fix-2/
categories:
  - Tips and Tricks

---
Firefox 1.5 brings up more unresponsive script warning on sites that use heavy Javascript like Gmail than the previous version. To fix this problem, you just have to change the configuration.

  * Type about:config in the address bar and you will get the hidden configuration page &#8211; similar to the windows registry editor.
  * In the filter box, type **dom.max\_script\_run_time**. This will filter the options and will display only the dom.max\_script\_run_time.
  * Right-click it and choose **Modify**. A box pops up. Change the number to something bigger like 20. This is the maximum time a script can run before Firefox considers it