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

#### Blockquotes
Blockquotes, as already used to show the output of previous code, places emphasis on a section of text. They are initiated using the \> marker and can be nested via \>\> ect.
``` markdown
  $ > Some text. <br />
  $ > Some more text. <br />
  $ >> Some nested text. <br />
```
> Some text. <br />
> Some more text. <br />
>> Some nested text. <br />

#### Lists
There are ordered and unordered lists, which can also be nested.
``` markdown
  $ 1. Item 1
  $ 1. Item 2
  $ 1. Item 3
  $    1. Nested item 1
  $    1. Nested item 2
  $ 1. Item 4
```
> 1. Item 1
> 1. Item 2
> 1. Item 3
>    1. Nested item 1
>    1. Nested item 2
> 1. Item 4

``` markdown
  $ - Item 1
  $ - Item 2
  $ - Item 3
  $   - Nested item 1
  $   - Nested item 2
  $ - Item 4
```
> - Item 1
> - Item 2
> - Item 3
>   - Nested item 1
>   - Nested item 2
> - Item 4

You can also use \* and \+ for lists and they can also be mixed.
``` markdown
  $ - Item 1
  $ + Item 2
  $ * Item 3
```
> - Item 1
> + Item 2
>   * Nested item 1
> * Item 3

A block of text can be within a list, providing the indentation is preserved.
``` markdown
  $ - Item 1
  $   
  $   Continue
  $ + Item 2
  $ *
```
> - Item 1
>   
>   continue
> - Item 2
> - Item 3

#### Code Blocks
Code with syntax highlight can be shown for a variety of languages. Encase code in backticks \` and specify a supported language for correct highlighting.
```
  $ ``` c
  $   void add(int a, int b) {
  $     int c;
  $     c = a + b;
  $     return c;
  $   }
  $ ```
```

``` c
  int add(int a, int b) {
  int c;
  c = a + b;
  return c;
  }
```

```
  $ ``` python
  $   def add(a, b):
  $     int c
  $     c = a + b
  $     return c
  $ ```
```
``` python
  def add(a, b):
    int c
    c = a + b
    return c
```

#### Images
Images from either local files or HTML links can be included within documents. The general syntax is:
``` markdown
  $ ![Image Name](path/to/file.png or HTML link)
```
> ![Markdown Logo](https://markdown-here.com/img/icon256.png)

#### Horizontal Rule
To section off documents, you can use horizontal rules. There are three ways of implementing this and all produce the same result.
``` markdown
  $ ***
  $ ===
  $ ___
```
> ***
> ---
> ___

#### Links
You can link to external webpages, such as my [GitHub](https://github.com/alexgregory1997).
``` markdown
  $ [word(s) to represent link](HTML link)
```
> This is a [link](https://github.com/alexgregory1997).

Further, the title of the link can be specified. This will appear when hovering over the link. <br />
``` markdown
  $ [word(s) to represent link](HTML link "Link Title")
```
> This is a [link](https://github.com/alexgregory1997 "Link Title"). <br />

Alternatively, a link or email can be linked by enclosing the URL or email address in angled brackets <example-email@gmail.com>.
``` markdown
  $ <example-email@gmail.com>
```
> <example-email@gmail.com>

They can also be formatted like text, hence enclosing in \* and \*\* will make it *<example-email@gmail.com>* and **<example-email@gmail.com>** respectively.

#### Referencing
Markdown allows formatted references, although they must be manually ordered.
``` markdown
  $ This is some reference in the text [name-reference][1] <br />
  $ [1]: <some-link> "Link Title"
```

> This is some reference in the text [name-reference][1] <br />
> <br />
> [1]: <some-link> "Link Title"

You can also include footnotes.
``` markdown
  $ This is some footnote [^1].
  $ [^1]: This is the contents of the footnote.
```
> This is some footnote [^1]. <br />
> <br />
> [^1]: This is the contents of the footnote.
