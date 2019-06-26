## Markdown Reference Notes
<p>The following document contains some basic notes on using Markdown. This is simply to serve as a quick reference guide for myself and any others who may find it useful.</p>

### Introduction to Markdown
<p>Include a brief summary of what Markdown is, the benefits and how it works. Note: the $ sign represents a new line.</p>

---

### General Markdown
#### Headers
There are six header levels defined by the number of \# signs.
``` markdown
  $ # Header 1
  $ ## Header 2
  $ ### Header 3
  $ #### Header 4
  $ ##### Header 5
  $ ###### Header 6
```
> # Header 1
> ## Header 2
> ### Header 3
> #### Header 4
> ##### Header 5
> ###### Header 6

There is an alternative syntax for header level 1 and 2, which is initiated by underlining with either '\=' (1) or '\-' (2).
``` markdown
  $ Header 1
  $ ========
  $ Header 2
  $ --------
```
> Header 1
> ========
> Header 2
> --------

#### Paragraphs and Line Breaks
Paragraphs can be defined by using <p\> and </p\> markers.
``` markdown
  $ <p>Some text.</p>
```
> <p>Some text.</p>

Line breaks can be specified using the <br /\> marker.
``` markdown
  $ First line of text. <br /> Second line of text.
```
> First line of text. <br /> Second line of text.

#### Comments
To add comments to .md files, simply use the <\!-- and --> markers.
``` markdown
  $ <!-- This is a comment -->
  $ This is not a comment
```
> <!-- This is a comment -->
> This is not a comment

#### Emphasis
For emphasis, text can be made __BOLD__, _ITALIC_, ~~STRIKETHROUGH~~ and a mixture, such as **_BOLD ITALICS_**.
``` markdown
  $ __BOLD__
  $ **BOLD**
  $ _ITALIC_
  $ *ITALIC*
  $ ~~STRIKETHROUGH~~
  $ **_BOLD ITALICS_**
```
> __BOLD__ <br />
> **BOLD** <br />
> _ITALIC_ <br />
> *ITALIC* <br />
> ~~STRIKETHROUGH~~ <br />
> **_BOLD ITALICS_** <br />
