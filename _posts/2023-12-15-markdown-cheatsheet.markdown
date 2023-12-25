---
layout:     post
title:      "Markdown Overview"
subtitle:   " \"Markdown Syntax Cheatsheet\""
date:       2023-12-15 12:00:00
author:     "Sebastian Sonne"
header-img: "img/in-post/md_example.png"
catalog: true
tags:
    - markdown
    - syntax
    - code
---

This is a basic cheatsheet for writing in Markdown. 

### Headers
<hr>
To create a header, use `#` for a level 1 header, `##` for level 2, and so on up to `######` for level 6.

```markdown
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

### Emphasis
<hr>
* *Italicize* text with `*asterisks*` or `_underscores_`.
* **Bold** text with `**double asterisks**` or `__double underscores__`.
* **_Combine them_** for `**_italic and bold_**`.
* ~~Cross out~~ text with `~double tilde~~`.

```markdown
*Italic* or _Italic_
**Bold** or __Bold__
**_Combined Emphasis_**
~~Strikethrough~~
```

### Lists
<hr>
#### Unordered Lists
Use `-` or `*` for bullet points.

```markdown
* Item 1
- Item 2
  * Sub Item 2.1
  - Sub Item 2.2
```
- Item 1
- Item 2
  - Sub Item 2.1
  - Sub Item 2.2

#### Ordered Lists
Use numbers followed by a period for an ordered list.

```markdown
1. First Item
2. Second Item
   1. Sub Item 2.1
   2. Sub Item 2.2
```
1. First Item
2. Second Item
   1. Sub Item 2.1
   2. Sub Item 2.2

### Links
<hr>
Create a link with `[link text](URL)`.

```markdown
This is an [example link](http://example.com).
```
This is an [example link](http://sebastian-sonne.github.io/2023/12/15/Hello-world/#links).

### Images
<hr>
Add images with `![Alt Text](image URL "Optional Title")`.

```markdown
![Alt text](http://example.com/image.jpg "Optional title")
```
![Alt text](/img/in-post/md_example_light.png "Optional title")

### Code
<hr>
#### Inline Code
Use backticks \` to format text as code inline.

```markdown
Inline `code` has `back-ticks around` it.
```

#### Code Blocks
Use triple backticks for a block of code. Optionally, specify the language for syntax highlighting.

```markdown
    ```javascript
    console.log("Hello, world!");
    ```
```
This is how it will look like:
```javascript
console.log("Hello, world!");
```

### Tables
<hr>
Create tables using `|` for columns and `-` for headers.

```markdown
| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| Row 1    | Data     | Details  |
| Row 2    | Data     | Details  |
```

| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| Row 1    | Data     | Details  |
| Row 2    | Data     | Details  |

### Blockquotes
<hr>
Use `>` for blockquotes. For nested blockquotes, use multiple `>`.

```markdown
> Lorem ipsum dolor sit amet.
>> Nested Blockquote.
```
> Lorem ipsum dolor sit amet.
>> Nested Blockquote.

### Horizontal Rule
<hr>
Use `---` for a horizontal rule.

```markdown
---
```
---
It is important to note that not all markdown renderers support all features. Some features might not work differently or are not available at all. Always test your markdown in its final display environment to ensure compatibility.

Happy Coding!

