# Markdown Docs & Notes <!-- omit from toc -->


## Headings

A space is required after the **hash** character:

# \# H1 <!-- omit from toc -->
## \#\# H2 <!-- omit from toc -->
### \#\#\# H3 <!-- omit from toc -->
#### \#\#\#\# H4 <!-- omit from toc -->
##### \#\#\#\#\# H5 <!-- omit from toc -->
###### \#\#\#\#\#\# H6 <!-- omit from toc -->


## Paragraphs and line breaks

Paragraphs need spacing before and after them.

Another paragraph with a \<br\><br>
this should be the next line.

If html tags are forbidden, use two trailing spaces to break a line  
here is the next line.


## Typography

*Italic* - **Bold** - <mark>highlight</mark> - x<sup>2</sup> - H<sub>2</sub>O

Depending from the location, it may be necessary to escape the following special characters with a **leading backslash**:  
\\ \` \* \_ \{\} \[\] \<\> \(\) \# \+ \- \. \! \|

Use **unicode** symbols with copy/paste:  
💣 🚀 ❤️ → 🙂

> Blockquote text
> - Item1
> - Item2
>> *Nested* one


## Horizontal rules

A horizontal rule gets added by 3 or more hyphens:

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
    # or one tab (no syntax highlighting)
    echo "Hello World!"
    printf ''%s\n' "$var1"

```bash
# 3-backticks code blocks support syntax highlighting:
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

- Shows up in HTML source code output: `<!-- Comment -->`

<!-- Comment -->

- Does not show up in HTML source code output: `[Comment]: #`

[Comment]: #


## Tables

| Head1 (left-align) | Head2 (centered) | Head3 (right-align) |
| :----------------  | :--------------: | ------------------: |
| Text1              | Text2            |               Text3 |
| Text4              | Text5            |               Text6 |


## Links

The path of the link is relative to the current file. In GitHub links starting with a slash are relative to the repository root.

### External links

[External link to contaware.com](https://www.contaware.com "Optional link title")

### Reference links

Reference links are useful when linking multiple times to the same target:

[First ref link to contaware.com][ref1]

[Second ref link to contaware.com][ref1]

[ref1]: https://www.contaware.com "Optional link title"

### Internal link

The anchors are derived from the headers like:

1. Making all letters lowercase
2. Numbers remain as they are
3. Spaces are replaced by hyphens
4. All other characters are removed

[Internal link](#headings)

### Link to another markdown file

[Link to another md file](another.md)

### Image

![alt text](contaware-header.png "Optional image title")

### Clickable image

[![alt text](contaware-header.png)](https://www.contaware.com)

### Image size

The Markdown syntax for images does not allow image width and height, use html if supported:

<img src="contaware-header.png" width="300" height="52" alt="alt text">
