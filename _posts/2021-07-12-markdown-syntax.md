---
title: "Markdown Syntax for blog"
excerpt: "HTML tags and formatting for blog - jekyll: minimal mistakes theme"

categories:
  - coding
tags:
  - [blog, github, markdown, jekyll, minimal mistakes theme]

toc: true
toc_sticky: true
 
date: 2021-07-12
last_modified_at: 2021-07-25
---

## Header
```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

## Line Break
### ▶️ `<br>`
Hello <br /> This is Areum
```
Hello <br /> This is Areum
```
### ▶️ two extra spaces + enter
end a line with two or more spaces, and then type return
```
Hello  
This is Areum
```

## Text Emphasis
### ▶️ Bold
I just love **bold text**.
```
I just love **bold text**.
```
### ▶️ Italic
add one asterisk or underscore before and after a word or phrase

Italicized text is the *cat's meow*.
```
Italicized text is the *cat's meow*.

Italicized text is the _cat's meow_.
```

## Blockquotes
### ▶️ Single line
> single line

```
> single line
```
### ▶️ multiple line
> multiple line: Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.

```
> multiple line: Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
```
### ▶️ nested Blockquotes
> Blockquotes
  >> nested Blockquotes

```
> Blockquotes
  >> nested Blockquotes
```
### ▶️ Blockquotes with Other Elements

> The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
```

## Cite reference
<cite>Steve Jobs</cite> --- Apple Worldwide Developers' Conference, 1997
{: .small}
```
<cite>Steve Jobs</cite> --- Apple Worldwide Developers' Conference, 1997
{: .small}
```

## Code Blocks
### ▶️ single line or word
To denote a word or phrase as code, enclose it in backticks (`)

`console.log('test')`

### ▶️ muttiple lines
enclose it in triple backticks (```)
```html
<html>
  <head>
  </head>
</html>
```

## Table
- Horizontal align
  - Left: `|:—|`
  - Center: `|:—:|`
  - Right: `|—:|`

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| a   | b   | c   |
| 1   | 2   | 3   |
|=============================|
| Foot1   | Foot2   | Foot3   |

```
| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| a   | b   | c   |
| 1   | 2   | 3   |
|=============================|
| Foot1   | Foot2   | Foot3   |
```

## List
### ▶️ Unordered Lists (Nested)

* List item one 
    * List item one 
        * List item one
        * List item two
    * List item two
    * List item three
* List item two
* List item three

```
* List item one 
    * List item one 
        * List item one
        * List item two
    * List item two
    * List item three
* List item two
* List item three
```
### ▶️ Ordered List (Nested)

1. List item one 
    1. List item one 
        1. List item one
        2. List item two
    2. List item two
2. List item two
3. List item three

```
1. List item one 
    1. List item one 
        1. List item one
        2. List item two
    2. List item two
2. List item two
3. List item three
```

## Notices

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice}` class.
{: .notice}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--primary}` class.
{: .notice--primary}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--info}` class.
{: .notice--info}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--warning}` class.
{: .notice--warning}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--success}` class.
{: .notice--success}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--danger}` class.
{: .notice--danger}

Change `{: .notice}` class to whatever you want - such as `{: .notice--info}`, `{: .notice--success}` etc.
```
**Watch out!** This paragraph of text has been [emphasized](#) with the notice class.
{: .notice}

**Watch out!** This paragraph of text has been [emphasized](#) with the notice class.
{: .notice--danger}
```

## Button
### ▶️ Color

[Default Button Text](#link){: .btn}
[Primary Button Text](#link){: .btn .btn--primary}
[Success Button Text](#link){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}

```
[Default Button Text](#link){: .btn}
[Primary Button Text](#link){: .btn .btn--primary}
[Success Button Text](#link){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}
```
### ▶️ Size

[X-Large Button](#link){: .btn .btn--primary .btn--x-large}
[Large Button](#link){: .btn .btn--primary .btn--large}
[Default Button](#link){: .btn .btn--primary }
[Small Button](#link){: .btn .btn--primary .btn--small}

```
[X-Large Button](#link){: .btn .btn--primary .btn--x-large}
[Large Button](#link){: .btn .btn--primary .btn--large}
[Default Button](#link){: .btn .btn--primary }
[Small Button](#link){: .btn .btn--primary .btn--small}
```

## Links

This is my [github](https://github.com/AreumAn "Areum An github")

```
This is my [github](https://github.com/AreumAn "Areum An github")
```

"Areum An github" is a title of link but you don't need to add.

```
This is my [github](https://github.com/AreumAn)
```
To quickly turn a URL or email address into a link, enclose it in angle brackets.
<https://github.com/AreumAn>
<fake@example.com>

```
<https://github.com/AreumAn>
<fake@example.com>
```

## Images

```
![alt text](/assets/images/test.png "image title")
```
### ▶️ Linking Images
```
[![alt text](/assets/images/test.jpg "image title")](url)
```


## 📚 Reference

**Reference list**  
<cite>[Basic Syntax]</cite> - <https://www.markdownguide.org/basic-syntax/>{: .small}  
<cite>[Markup: HTML Tags and Formatting]</cite> - <https://mmistakes.github.io/minimal-mistakes/markup/markup-html-tags-and-formatting/>{: .small}
{: .notice}
