Markdown: Let's Begin
=====================

## Table of Contents
[Basics](begin.md#Basics)
[Lists](begin.md#Lists)
[Links](begin.md#Links)


## Basics

### Paragraphs

Creating a new paragraph is relatively easy. All you have to do is just start writing on a new line.

Example:
```
You can write anything you want.

If you leave a blank space between the line, you will have a line break when you view the file. 
```

You can write anything you want.

If you leave a blank space between the line, you will have a line break when you view the file. 


### Headings

Like in HTML, we have six headers we can use. Instead of ```h1``` through ```h6``` tags, we have # tags.

```
# Represents h1 (or largest header)
## Represents h2
...
###### Represents h6
```
# Represents h1
## Represents h2
### Represents h3
#### Represents h4
##### Represents h5
###### Represents h6

### Blockquotes

This can be indicated with a ```>``` symbol before starting your quote.
```
Maya Angelou once said the following:

> Courage is the most important of all the virtues, because without courage you can't practice any other virtue consistently. You can practice any virtue erratically, but nothing consistently without courage.
```
Maya Angelou once said the following:

> Courage is the most important of all the virtues, because without courage you can't practice any other virtue consistently. You can practice any virtue erratically, but nothing consistently without courage.

### Styling Text

We can style our text to be *bold* or **italic**.
```
To add bold words, wrap your word(s) in "*" symbol, e.g. *bold text*

To add italics, wrap your word(s) in two "*" symbols, e.g. **italic text**

You may have italics with a bold phrase inside. No worries, use an underscore "_" to mean one or another. 

For example, **this phrase is in bold, _and this is in bold and italics_ to demostrate my point.**
```
*bold text*

**italic text**

For example, **this phrase is in bold, _and this is in bold and italics_ to demostrate my point.**

## Lists

### Unordered Lists

Use the ```*``` or ```-``` symbol in front of list. Be sure that this is the first character of the line. Do not add line breaks between the list items, which is unlike making a new paragraph.

```
* Item
* Item
* Item
or
- Item
- Item
- Item
```

* Item
* Item
* Item

### Ordered Lists

For ordered lists, you will want to add a number before the item. Like unordered lists, include the number and a period first and don't add line breaks.

```
1. Item 1
2. Item 2
3. Item 3
```

1. Item 1
2. Item 2
3. Item 3

## Links

### Inline Links

Create inline links by adding brackets ```[ ]``` around the text you want to link to and add the url link between parenthesis ```( )``` leading to the link. the brackets and parenthesis need to be next to each other, meaning no spaces between each other.

```
The best way to practice is to [visit GitHub!](www.github.com).
```

The best way to practice is to [visit GitHub!](www.github.com).

## Github Flavored Markdown

Github includes some more things that the original markdown does not have.

### Relative Link Paths

One of the cool things Github provides in their version of markdown is the use of [relative links](https://help.github.com/articles/relative-links-in-readmes). For example, I needed to include a button that goes back to the home page, so I added a link at the top that says "Back To Home". 

```
[Back To Home](../README.md)
```

[Back To Home](../README.md)



