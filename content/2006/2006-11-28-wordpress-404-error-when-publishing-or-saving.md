---
title: WordPress 404 error when publishing or saving

date: 2006-11-28
url: /2006/11/28/wordpress-404-error-when-publishing-or-saving/
categories:
  - Software
  - Tips and Tricks

---
<img align="left" id="image299" alt="Wordpress logo" src="http://www.fslog.com/wp-content/uploads/2006/11/wordpress-logo-cristal.thumbnail.jpg" />WordPress has this particular problem when publishing or saving a blog post where it shows a 404 page instead of the required effect. This is irritating when you have typed a long post and just after you have published it shows the 404 error, and all your data is lost. I have faced this same problem for many times.
  
After a bit of Googling, I found out that the problem is with mod_security being set on server.
  
To fix this, add the following two lines in our .htaccess file.
  
`SecFilterEngine Off<br />
SecFilterScanPOST Off`

This should fix the problem. Let me try publishing this post.