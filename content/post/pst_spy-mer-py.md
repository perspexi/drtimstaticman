+++
title = "Mercurial, Spyder/Python(x,y) and Windows 7"
slug = "spy-mer-py"
date = 2012-12-15
lastmod = 2012-12-15
draft = false
#math = true
#markup = "mmark"
tags = []
summary = "How to tag matplotlib figures with the Mercurial repo. version"
#[header]
#image = "headers/sunset.png"
#caption = "Image: [**Sunset at Kamouraska**](https://commons.wikimedia.org/wiki/File:Sunset_at_Kamouraska.jpg)"
## create a gallery
#[[gallery_item]]
#album = "1"
#image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-default.png"
#caption = "Default"
+++

Spyder supports mercurial or SVN. The 1st thing is to install Mercurial in Windows. Easy enough. Make the dir containing the code into a Mercurial working dir. Fine. Now try to commit it to the local repository...  hg complains, something about the user. It's the windows install. The fix:  make an hgrc file in the .hg directory. now add this to the file:
```yaml
	[ui]
	username = Some Lass <saucy@nomail.com>
	verbose = True
```
Now spyder can recognize the hg working dir. Now enable the keyword extension
```yaml
	[extensions]
	keyword=
	#or, if keyword.py is not in the hgext folder:
	#keyword=/path/to/keyword.py
```
And add some other stuff
```yaml
	# filename patterns for expansion are configured in this section
	[keyword]
	# expand keywords in all python files in working dir
	**.py =
	# do not expand keywords in files matching "x*" in working dir
	x* = ignore
	# override the cvs-like default mappings with customized keyword = expansion pairs,
	# where expansion values contain Mercurial templates and filters
	[keywordmaps]
	HGdate = {date|rfc822date}
	lastlog = {desc}
	checked in by = {author}
	Id = v {node|short} {date|utcdate} {author|user}
```
Now include the code in a python file
```python
	hgid = '$Id: $'
	hgid = hgid[4:-1]
```
when you commit, it will expand to something like
```python
	hgid = '$Id: ecbase.py,v 37ea39143d90 2012/09/01 22:32:27 tim $'
	hgid = hgid[4:-1]
```
and voila, you have a id tag in your code for including on plot graphics. now you can reproduce any plot in a matter of minutes, provided the data's in the same stop and you commit each time before you make plots

