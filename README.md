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

- `*Italic*` *Italic*
- `**Bold**` **Bold**
- `~~Strikethrough~~` ~~Strikethrough~~

If html tags are supported:

- `<mark>highlight</mark>` <mark>highlight</mark> 
- `x<sup>2</sup>` x<sup>2</sup>
- `H<sub>2</sub>O` H<sub>2</sub>O 
- `<small>small</small>` <small>small</small>

Depending from the location, it may be necessary to escape the following special characters with a **leading backslash**:  
\\ \` \* \~ \_ \{\} \[\] \<\> \(\) \# \+ \- \. \! \| \$

Use **unicode** symbols with copy/paste:  
💣 🚀 ❤️ → 🙂

> \> Blockquote text


## Horizontal rules

A horizontal rule gets added by **3 or more hyphens**:

---


## Lists

Unordered list items start with one of `- * +` and order list items with a **number followed by a dot**. List subitems have to indent at least as much as the first character that's not part of the list marker and not a whitespace. For unordered lists that's 2 and for ordered lists that's 3 or 4 if you hit the `10.` list marker.

```
- Item1
  * SubItem1
    + SubSubItem1
- Item2
```

- Item1
  * SubItem1
    + SubSubItem1
- Item2

```
1. Item1
   1. SubItem1
      1. SubSubItem1
2. Item2
```

1. Item1
   1. SubItem1
      1. SubSubItem1
2. Item2


## Task lists

Task lists are supported by some markdown flavors, they are sometimes also called check lists or todo lists:

```
- [ ] unchecked
- [x] checked
```

- [ ] unchecked
- [x] checked
  

## Inline code

- Enclose `inline code` in **backticks**.

- Enclose `` inline code containing `backtick(s)` `` in **double-backticks**.  
  Note: the backtick delimiters surrounding an inline code may include one space after the opening and one before the closing to allow placing literal backticks at the beginning or end of an inline code.


## Code blocks

    # Traditional code blocks with four leading spaces
    # or one tab (no syntax highlighting)
    echo "Hello World!"
    printf '%s\n' "$var1"

```bash
# 3-backticks code blocks support syntax highlighting:
# c cpp arduino|ino csharp javascript|js json html css
# php python|py bash powershell|ps markdown|md
echo "Hello World!"
printf '%s\n' "$var1"
```

```console
# Some markdown renderers do color the prompt when
# providing console as the syntax highlighting language
foo@bar:~$ git --version
```


## Comments

- Shows up in html source code output: `<!-- Comment -->`

<!-- Comment -->

- Does not show up in html source code output: `[Comment]: #`

[Comment]: #


## Tables

```md
| Left align  | Centered | Right align |
| :---------  | :------: | ----------: |
| T1          | T2       | T3          |
| T4          | T5       | T6          |
```

| Left align  | Centered | Right align |
| :---------  | :------: | ----------: |
| T1          | T2       | T3          |
| T4          | T5       | T6          |


## Links

The path of a link is relative to the current file. In GitHub links starting with a slash are relative to the repository root.

### External links

```md
[Link](https://www.contaware.com "Optional Title")

<https://www.contaware.com>
```

[Link](https://www.contaware.com "Optional Title")

<https://www.contaware.com>

### Reference links

Reference links are useful when linking multiple times to the same target.

```md
[First Link][ref1]

[Second Link][ref1]

[ref1]: https://www.contaware.com "Optional Title"
```

[First Link][ref1]

[Second Link][ref1]

[ref1]: https://www.contaware.com "Optional Title"

### Email links

```md
[Contact Us](mailto:oliver.pfister@contaware.com)

<oliver.pfister@contaware.com>
```

[Contact Us](mailto:oliver.pfister@contaware.com)

<oliver.pfister@contaware.com>

### Internal links

The anchors are derived from the headers like:

1. Making all letters lowercase
2. Numbers remain as they are
3. Spaces are replaced by hyphens
4. All other characters are removed

```md
[Internal link](#headings)
```

[Internal link](#headings)

### Link to another markdown file

```md
[Link to another md file](another.md)
```

[Link to another md file](another.md)

### Image

Big images are automatically scaled to fit the page width.

```md
![alt text](figures/contaware-header.png "Optional Title")
```

![alt text](figures/contaware-header.png "Optional Title")

### Clickable image

```md
[![alt text](figures/contaware-header.png)](https://www.contaware.com)
```

[![alt text](figures/contaware-header.png)](https://www.contaware.com)


## Math

LaTeX formatted math is supported by some markdown flavors.

- Surround an inline math expression with single-dollar symbols: `$x^2$` $x^2$

- Make math blocks by enclosing them in double-dollar symbols:

  ```
  $$P = 2\pi r$$
  
  $$A = \pi r^2$$
  ```

  $$P = 2\pi r$$
  
  $$A = \pi r^2$$
