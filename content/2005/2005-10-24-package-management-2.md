---
title: Package Management

date: 2005-10-24
url: /2005/10/24/package-management-2/
categories:
  - Software
  - Tutorial

---
Applications for GNU/Linux are available in various formats like source(.tar.gz), deb, rpm. In my opinion Debian&#8217;s package management is far superior than others as it automatically checks for dependancy packages and installs them too(there is _yum_ forRedHat, but I don&#8217;t use RedHat).
  
You can install/update/remove packages using **synaptic package manager**. Open synaptic from **System>Administration>Synaptic Package Manager**.
  
You can find the interface easy to use. Just select your package at the upper-right corner and click the tick box. Synaptic automatically installs the dependency packages too if required.
  
So you may be asking from where does synaptic install the software. There are various repositories on the net that is used by synaptic to install or update the system. Usually we use the command line tools to install them, but synaptic gives a easy to use interface.
  
You can view the repositories or add new ones by going to the **Settings>Repositories** menu and a list of repositories are shown. Click settings and tick the Show Disabled software sources.
  
You can now see checkboxes next to the repositories.
  
Enable the Universe repository. You can also enable the Multiverse and the Universe Security updates repository. Save the changes.
  
You need to update the packages to obtain the list of packages in the repository.
  
After this, you can install the packages.

You can also add new Repositories. For eg
  
deb http://www.grawert.net/ubuntu/ warty universe
  
Here the various fields are
  
deb &#8211; neaning it is a binary
  
http://www.grawert.net/ubuntu/ &#8211; URi(Uniform Resource Identifier) which is the location of the repository
  
warty &#8211; the release name
  
universe &#8211; section name. There can be several sections seperated by a space.

Hope you have got a nice overview of the package management in Ubuntu.

<div>
  Tech Tags: ubuntu linux <a rel="tag" href="http://technorati.com/tag/gnu/linux">gnu/linux</a> <a rel="tag" href="http://technorati.com/tag/repository">repository</a> <a rel="tag" href="http://technorati.com/tag/deb">deb</a> <a rel="tag" href="http://technorati.com/tag/apt">apt</a> synaptic <a rel="tag" href="http://technorati.com/tag/breezy">breezy</a>
</div>