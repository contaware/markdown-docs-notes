# Markdown Docs & Notes <!-- omit from toc -->

## Table of contents <!-- omit from toc -->

- [Headings](#headings)
- [Paragraphs and line breaks](#paragraphs-and-line-breaks)
- [Typography](#typography)
- [Horizontal rules](#horizontal-rules)
- [Lists](#lists)
- [Code](#code)
- [Comments](#comments)
- [Tables](#tables)
- [Links](#links)


## Headings

A space is required after the hash!

# H1 <!-- omit from toc -->
## H2 <!-- omit from toc -->
### H3 <!-- omit from toc -->
#### H4 <!-- omit from toc -->
##### H5 <!-- omit from toc -->
###### H6 <!-- omit from toc -->


## Paragraphs and line breaks

Paragraphs need spacing before and after them.

Another paragraph with a \<br\><br>
this should be the next line.

If html tags are forbidden use two trailing spaces to break a line  
here is the next line.


## Typography

*Italic* - **Bold** - <mark>highlight</mark> - x<sup>2</sup> - H<sub>2</sub>O

Escape special chars with backslashes: \*Normal\*

Use unicode symbols with copy/paste: 💣 🚀 ❤️ → 🙂

> Blockquote text
> - Item1
> - Item2
>> *Nested* one


## Horizontal rules

---


## Lists

List subitems have to indent at least as much as the first character that's not part of the list marker and not a whitespace. For unordered lists that's 2 and for ordered lists that's 3 or 4 if you hit the 10. list marker.

- Item1
  * SubItem1
  * SubItem2
- Item2
- Item3

1. Item1
   1. SubItem1
   2. SubItem2
2. Item2
3. Item3


## Code

This is a `inline code` with backticks. 

    # Traditional code blocks with four leading spaces
    # or one tab (not syntax highlighting)
    echo "Hello World!"
    printf ''%s\n' "$var1"

```bash
# 3-backticks code blocks support languages for syntax highlighting:
# c cpp arduino|ino csharp javascript|js json html css php 
# python|py bash powershell|ps markdown|md
echo "Hello World!"
printf ''%s\n' "$var1"
```

```console
# Some markdown renderers with the console language
# will also highlight the prompt
foo@bar:~$ git --version
```


## Comments

- Shows up in a HTML source code output: `<!-- Comment -->`

<!-- Comment -->

- Does not show up in a HTML source code output: `[Comment]: #`

[Comment]: #


## Tables

| Head1 (left-align) | Head2 (centered) | Head3 (right-align) |
| :----------------  | :--------------: | ------------------: |
| Text1              | Text2            |               Text3 |
| Text4              | Text5            |               Text6 |


## Links

The path of the link is relative to the current file. In GitHub links starting with a slash are relative to the repository root.

[Contaware](https://www.contaware.com "Optional link title")

[Link to Headings](#headings)

[Link to another md file](another.md)

[Ref link][ref1]

![alt text](image.jpg "Optional image title")

[![alt text](image.jpg)](https://www.contaware.com)

The Markdown syntax for images doesn't allow image width and height, use html:

<img src="https://www.contaware.com/images/headers/contaware_header.png" width="600" height="100" alt="alt text">

[ref1]: https://www.google.com "Optional link title"
