Markdown: Let's Begin
=====================
[Back To Markdown Home Page](readme.md)

## Table of Contents
1. [Basics](#basics)
	1. [Paragraphs](#paragraph)
	2. [Headings](#heading)
	3. [Blockquotes](#block)
	4. [Codeblocks](#code)
	5. [Styling Text](#style)
	6. [Horizontal Rule](#horizontal)
2. [Lists](#lists)
3. [Links](#links)
4. [Github Flavored Markdown](#github)
5. [Writing in Github](#writing)

<a name="basics"/>
## Basics

<a name="paragraph"/>
### Paragraphs

Creating a new paragraph is relatively easy. All you have to do is just start writing on a new line.

Example:
```
You can write anything you want.

If you leave a blank space between the line, you will have a line break when you view the file. 
```

You can write anything you want.

If you leave a blank space between the line, you will have a line break when you view the file. 

<a name="heading"/>
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

We also use ```=``` and ```-``` lines underneath h1 and h2 headings.

```
Heading 1
=========

Heading 2
---------
```

Heading 1
=========

Heading 2
---------

<a name="block"/>
### Blockquotes

This can be indicated with a ```>``` symbol before starting your quote. You can still use other markdown features within the quotes.
```
Maya Angelou once said the following:

> Courage is the most important of all the virtues, because without courage you can't practice any other virtue consistently. You can practice any virtue erratically, but nothing consistently without courage.
```
Maya Angelou once said the following:

> Courage is the most important of all the virtues, because without courage you can't practice any other virtue consistently. You can practice any virtue erratically, but nothing consistently without courage.

We can also nest blockquotes.

```
> Normal Quote

>> Nested Quote in Normal Quote

> End of Normal Quote
```

> Normal Quote

>> Nested Quote in Normal Quote

> End of Normal Quote

<a name="code"/>
### Codeblocks

You can create a quick codeblock by indenting.

```
Normal Text

	Indented Quoted Text

Back to Normal Text
```

Normal Text

	Indented Quoted Text

Back to Normal Text

The more proper way of doing it is to start by putting three backticks ``` ` ``` symbols at the beginning and end of their code blocks. Putting the langauge after the three backticks allows for code highlighting.

	```ruby
	class Die
	  def initialize(labels)
	  	raise ArgumentError.new("No empty labels allowed") unless labels.length > 0
	  	@sides = labels
	  end

	  def sides
	  	@sides.length
	  end

	  def roll
	  	@sides.sample
	  end
	end
	```
```ruby
class Die
  def initialize(labels)
  	raise ArgumentError.new("No empty labels allowed") unless labels.length > 0
  	@sides = labels
  end

  def sides
  	@sides.length
  end

  def roll
  	@sides.sample
  end
end
```

<a name="style"/>
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

<a name="horizontal"/>
### Horizontal Rule

Adding a horizontal rule requires three or more hyphens ```---```, asterisks ```***``` or underscores ```___``` on their own line.

```
---

***

___
```

---

***

___

<a name="lists"/>
## Lists

### Unordered Lists

Use the ```*``` or ```-``` or ```+``` symbol in front of list. Be sure that this is the first character of the line. Do not add line breaks between the list items, which is unlike making a new paragraph.

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

### Paragraphs within Lists

The following is from [this guide](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) taken line by line.

```no-highlight
1. First ordered list item
2. Another item
	* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
	1. Ordered sub-list
4. And another item.

	You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

	To have a line break without a paragraph, you will need to use two trailing spaces.  
	Note that this line is separate, but within the same paragraph.  
	(This is contrary to the typical GFM line break behavior, where trailing spaces are not required.)
```

1. First ordered list item
2. Another item
	* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
	1. Ordered sub-list
4. And another item.

	You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

	To have a line break without a paragraph, you will need to use two trailing spaces.  
	Note that this line is separate, but within the same paragraph.  
	(This is contrary to the typical GFM line break behavior, where trailing spaces are not required.)

<a name="links"/>
## Links

### Inline Links

Create inline links by adding brackets ```[ ]``` around the text you want to link to and add the url link between parenthesis ```( )``` leading to the link. the brackets and parenthesis need to be next to each other, meaning no spaces between each other.

```
[I'm an inline-style link to Github](https://www.github.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[This is a reference-style link][With Arbitrary case-insensitive reference text]

[You can use numbers (wow) for reference-style link definitions][1]

Or leave it empty and use the [link text itself]

Some text to show that the reference links can follow later.

(This following part won't show without blocking it out, so I added '>' signs in front. You don't normally add them)

>[with arbitrary case-insensitive reference text]: https://www.mozilla.org
>[1]: http://slashdot.org
>[link text itself]: http://www.reddit.com
```

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][with Arbitrary case-insensitive reference text]

[You can use numbers (wow) for reference-style link definitions][1]

Or leave it empty and use the [link text itself]

Some text to show that the reference links can follow later.

[with arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

<a name="github"/>
## Github Flavored Markdown

Github includes some more things that the original markdown does not have.

### Relative Link Paths

One of the cool things Github provides in their version of markdown is the use of [relative links](https://help.github.com/articles/relative-links-in-readmes). For example, I needed to include a button that goes back to the home page, so I added a link at the top that says "Back To Home". 

```
[Back To Home](../README.md)
```

[Back To Home](../README.md)

<a name="writing"/>
## Writing within Github vs. Markdown document

I've been writing on Sublime text, which is not the same as writing in markdown via Github when writing issues, comments, and pull request descriptions. Here are the notable differences.

### Newlines

No more empty new lines between paragraphs. Look at the following:
```
Farts and more farts
Separated into its own lines.
```

becomes:

Farts and more farts

Separated into its own lines.

### Task lists

TBA

### Features

All of these differences so far are mark-up differences. There are features includes as well, although it doesn't pertain to my learning since I'll be writing off in a text editor anyways. These include Quick Quoting, Team and Name @mention Autocompletions, Emoji autocomplete, Issue autocompletion, and Zen Mode (fullscreen) writing. If you're curious, please check out this page on '[Writing on Github](https://help.github.com/articles/writing-on-github)'.

## Resources:

* [Markdown Basics from Github](https://help.github.com/articles/markdown-basics)
* [Github Flavored Markdown](https://help.github.com/articles/github-flavored-markdown)
* [Writing on Github](https://help.github.com/articles/writing-on-github)
* [Daring Fireball: Markdown Basics](https://daringfireball.net/projects/markdown/basics)
* [Daring Fireball: Markdown Syntax](http://daringfireball.net/projects/markdown/syntax)
* [Adam Pritchard's Github Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

