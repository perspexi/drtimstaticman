+++
title = "Examples: Markdown (with mmark) and Hugo short codes"
date = 2016-04-20
lastmod = 2018-01-13
draft = true
math = true
markup = "mmark"
tags = ["mmark","example"]
summary = "Markdown (with mmark) and Shortcodes"
[header]
image = "headers/beachshell.jpg"
caption = "Image: [**Shell on the beach**](https://depositphotos.com/7100045/stock-photo-shell-on-the-beach.html)"
#create a gallery
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-default.png"
caption = "Default"
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-ocean.png"
caption = "Ocean"
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-dark.png"
caption = "Dark"
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-forest.png"
caption = "Default"
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-coffee-playfair.png"
caption = "Coffee theme with Playfair font"
[[gallery_item]]
album = "1"
image = "https://raw.githubusercontent.com/gcushen/hugo-academic/master/images/theme-1950s.png"
caption = "1950s"
+++
With mmark
# Heading 1 of 6
## Heading 2 of 6
### Heading 3 of 6
#### Heading 4 of 6
##### Heading 5 of 6
###### Heading 6 of 6
---
## Escaping Markdown/HTML (Writing Code)
Backticks make code: `&nbsp;`

    different code-like block quote
    &nbsp;
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
```python
s = "Python syntax highlighting"
print s
```

## Block quote
Some text. Default markdown requires an empty line before the block quote.
> a block quote &nbsp;

## Whitespace
Two spaces after a line renders a newline.  
One space after a new line 
does not.  
One empty line is rendered if one or more enpty lines follow a two space ending  
 
To force a space, the HTML non-breaking_space code (\&nbsp;) must be used:(&nbsp;)  
Tab also renders a space:(&Tab;)  
`&NewLine;` does not render a &NewLine; newline. 
Many more HTML symbols referenced at [Symbol Codes | Entity Codes for HTML](http://sites.psu.edu/symbolcodes/codehtml/)  
I'm not sure which id these codes are supported by hugo's default markdown and mmark markdown.  

## Formatting:
 *italic* _italic_ **bold** __bold__ ***bold_italics***  
sub~script~ super^script^ ~~strikethrough~~  
Dashes -- and --- (not rendered by mmark)  
Three consecutive dots ... into an ellipsis  
Fractions 1/2 1/3 3/4 (not rendered by mmark)  
There's no "proper" way to indent. You have to  
$\quad$ hack it with Latex. More ways are listed on [this stackoverflow post](https://stackoverflow.com/questions/6046263/how-to-indent-a-few-lines-in-markdown-markup)

## Symbols
Symbols (c), (tm), and (r) (not rendered by mmark)  
HTML symbols can come in handy: &sect; &yen; &cent; &pound; &euro; &curren;  
Some (like the Dutch Florin symbol: &fnof;) may work in older browsers.  
Unicode symbols work too.
¥,£,€,¤,ƒ  

## Links and Images:
Here is a [link](https://www.google.com) to google.  
An Image:
[![caption](https://raw.githubusercontent.com/gcushen/hugo-academic/master/academic.png)](https://github.com/gcushen/hugo-academic/)
## Latex
Works when "math = true" is added to gohugo page meta data. I think it's rendered by by [MathJax](https://www.mathjax.org/) ([quickref](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)). Some markdown implementaitons use [KaTeX](https://khan.github.io/KaTeX/).  
Inline $y=\text{m}x +\rm{b}$  
centered (mmark requires an empty preceeding line):

$$ y=\text{m}x +\rm{b} $$  

### Caveats

An empty line before a Latex block will add a barely noticeable bit of extra space than no empty line. 
empty line before kjhfoajh fojsf oijs ofijsiof jio

$$
y=\text{m}x +\rm{b}
$$  

no empty line kjhfoajh fojsf oijs ofijsiof jio. (N/A for mmark)
$$
y=\text{m}x +\rm{b}
$$  

## Lists

1. First ordered list item
2. Another item
You can have properly indented paragraphs within list items. 
3. Third item

---
Emojis:
:+1: :sparkles: :camel: :tada: :rocket:  
Some don't work: :metal: :octocat:  
[emoji codes](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

## Tables (colons align columns):
Some text. An empty line is required before the table.

Markdown | Less | Pretty
---|:---:|---:
*Still* | `renders` | **nicely**
1 | 2 | 3

## Youtube
Some text. Default opens a new window, mmark does not.
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/KmtzQCSh6xk/0.jpg)](http://www.youtube.com/watch?v=KmtzQCSh6xk)

## Comments
One way to comment (renders an empty line):
[//]: # ( a comment )
An HTML comment (can be multi-line):
<!-- this is a comment
with empty lines
-->  
More comments hacks are listed on [Stack Overflow](https://stackoverflow.com/questions/4823468/comments-in-markdown).

## Horizontal lines
Some text. An empty preceeding line is required.

---
Horizontal lines can be made with - or _ x3.  = or + may work for some markdown implementaitons, but dont seem to work for Hugo. The browser's soom level may play funny tricks on the appearance of horizontal lines. 

___

===

+++

## Other Examples
[Wordpress Markdown quick reference](https://en.support.wordpress.com/markdown-quick-reference/)

Below is a Hugo gallery.

{{< gallery >}}

