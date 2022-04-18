---
title: An Introduction to Markdown
author: Deborah Mundorff
---

# An Introduction to Markdown

This past February, I was putting together a proposal for the [2022 Distance Teaching & Learning (DT&L) Conference](https://conferences.upcea.edu/DTL2022/proposals.html?_zs=CcsHX&_zl=24ox2), and I shared my draft with a couple of my colleagues for feedback.

Typically, when requesting feedback, our team relies on Google Docs, which has a [nice feature set](https://support.google.com/docs/answer/6033474?hl=en&co=GENIE.Platform%3DDesktop) for suggesting edits.

However, I was not using Google Docs. I explained that they would be viewing my formatted document on [HackMD](https://hackmd.io/), a collaborative web-based Markdown tool.

One of the colleagues I had asked for feedback responded:

What are the pros and cons compared to a google doc, may I ask?

That question inspired this blog post.

## What is Markdown?

Markdown is a plain text format with a simple syntax to add formatting elements (headings, lists, quotes, bold, italics, etc.). It is easy to convert Markdown files into other formats, such as PDFs, HTML, and rich text. One of the primary uses of Markdown is creating content for the web, which can be done with almost no knowledge of HTML. The first [Markdown](https://en.wikipedia.org/wiki/Markdown) specification was developed by [John Gruber](https://daringfireball.net/projects/markdown/) and Aaron Swartz in 2004 and released as Open Source.

## What Are the Advantages of Writing in Markdown?

### It Is Easy to Learn and Fast to Write

Most markdown syntax is intuitive. Perhaps you are writing a document, and you decide you want to emphasize some text using bold or italics styling. In Markdown, you can surround the words with underscores or asterisks rather than select content and apply a style from a menu or keyboard command. For **bold** text, add either two asterisks or two underscores before and after the word (your choice, most editors support either syntax):

```Markdown
**bold**
__bold__
```

For text that you want to be displayed in italics, use one underscore or asterisk before and after the word:

```Markdown
*italics*
_italics_
```

Creating hyperlinks in documents, a somewhat tedious process in a word-processing program or HTML, is as easy as putting a descriptive link text in brackets and then an address immediately following in parenthesis, like this:

```Markdown
[OSU Canvas Dashboard](https://canvas.oregonstate.edu/)
```

which in my document becomes: [OSU Canvas Dashboard](https://canvas.oregonstate.edu/).

### It Is Just a Text File

A Markdown file with the extension ".md" is just a plain text file. Storing information in plain text files has several advantages:

1. Text files are future-proof. You can open a plain text file with any editor on any platform. You are not hostage to the proprietary format chosen by an application developer. You are not dependent on any particular software program still being around to open your Markdown files.
2. Text files require very little storage. This blog post, written in Markdown, was almost 250% larger once converted to a Microsoft Word document.
3. Text files are platform-agnostic, making them easy to share with other people or multiple devices. A text file can be opened on a Mac, on Windows, in Chrome OS, in a web browser, on an ios or Android smartphone, or on a Linux machine.
4. If you open up one of your Markdown text documents in platforms like Box or Dropbox, it automatically renders the HTML.

### Markdown is Highly Portable

One of the most significant advantages to writing in Markdown is how easy it is to convert Markdown into virtually any other file format:

* **HTML:** With no knowledge or experience in web development, you can quickly convert Markdown to HTML. There are many ways to convert Markdown to HTML. You can use a web-based tool such as [Markdown2Html](https://codebeautify.org/markdown-to-html) or [StackEdit](https://stackedit.io/) or work in a text editor with support for exporting Markdown in various formats like [Brackets](https://brackets.io/).
* **RTF:** An RTF file keeps basic formatting, such as links or emphasis, while retaining a text file's flexibility and small size.
* **PDFs:** Many Tools support applying CSS-based styles during a conversion. On my Mac, I use [Marked 2](https://marked2app.com/) and several of the [Marked 2 - Custom Styles](https://marked2app.com/styles/) to create beautiful PDF files.
* **Word:** Markdown formatting information (titles, headings, quotes, paragraphs, lists, etc.) is retained during conversion. Suppose you convert a document from Markdown to Word. You can then apply any of the [built-in styles](https://support.microsoft.com/en-us/office/customize-or-create-new-styles-d38d6e47-f6fc-48eb-a607-1eb120dec563) available in Microsoft Word to format your file instantly.

For a much longer list of the supported conversion file types, explore [Pandoc](https://pandoc.org/), a universal conversion utility. Using Pandoc, I have converted markdown files into a slide deck, a mind map, a Google Doc, and a Microsoft Word doc, but there are dozens of additional options.

### It Is Easier to Read and Write Than HTML

Let's look at a numbered list with some simple formatting. I have applied **bold** to item 1 and _italics_ to item 4:

1. **Analysis**
2. Design
3. Development
4. _Implementation_
5. Evaluation

Here is what that list looks like in Markdown:

```Markdown
1. **Analysis**
2. Design
3. Development
4. _Implementation_
5. Evaluation
```

If you were to write that same list in HTML, it would look like this:

```HTML
<ol>
<li><strong>Analysis</strong></li>
<li>Design</li>
<li>Development</li>
<li><em>Implementation</em></li>
<li>Evaluation</li>
</ol>
```

Even if you are comfortable coding in HTML, writing the list in Markdown is much quicker and can be quickly converted to HTML at any time.

### You Can Write Without Distraction

Using Markdown, I can focus on content rather than the formatting. I can indicate how something should be formatted (as a hyperlink, heading, paragraph, etc.) and then let a MarkDown tool transform my document to numerous other file types. I don't have to look at dozens of text and paragraph formatting options on a ribbon toolbar or interrupt my writing to apply them.

###

## What Do You Need to Get Started?

### A Text Editor

You can write Markdown in any text editor. However, many tools provide a real-time preview of your formatted document and give you several export options. These web-based Markdown tools are free options worth exploring:

* [Dillinger](https://dillinger.io/) is a great place to start. You can experiment with the syntax and instantly preview your content without installing any software on your computer. There is support for export to [StackEdit](https://stackedit.io/) works much the same way. Both are free, and both support export to HTML and PDF.
* [HackMD](https://hackmd.io/) is another web-based tool, also free, which has collaborations options.

If you prefer working in a desktop application, there are also many options. [Here is a nice write up of several Markdown Editors.](https://helpdeskgeek.com/free-tools-review/best-Markdown-editors-all-platforms-and-online/)

### Learning the Syntax

After choosing your editor, you need to get familiar with some basic syntax. The most common and helpful Markdown syntax is _very_ easy to master. You saw **bold**, _italics_, and a Markdown link earlier. Here are a few more examples:

#### **Headings**

To place a heading in the document, precede the text for the heading with one or more hashtags. Here's a level two heading:

## Level Two Heading

In Markdown, you would write it like this:

```Markdown
## Level Two Heading
```

Many Markdown editors also support the use of an id in a heading:

```Markdown
### Level Three Heading {#custom-id}
```

When converted to HTML, this will give you an anchor that you can use to link directly to that heading.

```html
<h3 id="custom-id">Level Three Heading</h3>
```

#### **Lists**

Lists look much like they would in any other document. Here is a numbered list:

1. trumpet
2. french horn
3. tubal
4. trombone

which in Markdown is:

```Markdown
1. trumpet
2. french horn
3. tuba
4. trombone
```

and an unordered list:

* cymbal
* drum
* marimba
* tambourine
* xylophone

looks like this in Markdown:

```Markdown
- cymbal
- drum
- marimba
- tambourine
- xylophone
```

Or you can use the single * with a space to make list items like this:

```Markdown
* string instruments
    * cello
    * violin
    * harp 
```

Note the support for indenting lists using spaces in the example above, which would work with either `*` or `-`. The Markdown list above would render like this:

* string instruments
  * cello
  * violin
  * harp

#### **Hyperlinks**

To make a hyperlink in Markdown, you write a descriptive title in brackets, followed by the URL in parenthesis, as mentioned above. You can even save yourself the trouble of manually creating markdown links through the use of one of the many available browser extensions [like this one for Chrome](https://chrome.google.com/webstore/detail/copy-title-and-url-as-mar/fpmbiocnfbjpajgeaicmnjnnokmkehil?hl=en) or [this one for Firefox](https://addons.mozilla.org/en-US/firefox/addon/copy-as-markdown/).

Rather than document the complete set of Markdown formatting options, I will refer you to the [Markdown Basic Syntax Guide](https://www.Markdownguide.org/basic-syntax/) or in Markdown:

```Markdown
[Markdown Basic Syntax Guide](https://www.Markdownguide.org/basic-syntax/)
```

## MultiMarkdown: An Expansion of the Language

The Markdown language is Open Source. Since its inception, other developers have enhanced the language to include options beneficial to academic writers. These include:

* tables
* blockquotes
* citations
* footnotes [^1]

Adding specific examples of these items is beyond this basic Markdown blog post. Instead, I recommend reviewing the [MultiMarkdown v6 Syntax Guide](https://rawgit.com/fletcher/MultiMarkdown-6-Syntax-Guide/master/index.html). As you will see, the syntax for the new items follows the same spirit of being easy to add to a document and relatively intuitive syntax.

## Advanced Tools and Applications

If you want to do a deep dive on Markdown, here are a few resources you can explore:

* [Pandoc](https://pandoc.org/MANUAL.html): a universal convert that will convert a markdown file to dozens of other formats.
* [Mac Power Users #548: Jumping Into Markdown - Relay FM](https://www.relay.fm/mpu/548)
* [Markdown Service Tools - BrettTerpstra.com](https://brettterpstra.com/projects/Markdown-service-tools/)
* [Markdown Tables generator - TablesGenerator.com](https://www.tablesgenerator.com/Markdown_tables)
* [Setting Up a Scholarly Writing Environment With Markdown, VSCodium, and pandoc](https://youtu.be/J86Pm62XM_Q)

## Yes, But What Are the Cons?

You may recall that my colleague asked about the pros _and_ the cons. So, as much as I love writing in Markdown, I should be transparent about the limitations I have encountered.

1. Collaboration. Both Microsoft Word and Google Docs support providing feedback on documents using the review or suggestion features. I have yet to find a Markdown editor that supports this type of collaboration. When I want to have a document reviewed, I convert the Markdown document to one of those other formats and then convert it back after implementing the feedback. Converting from Markdown _to_ something, as I have said, is something most markdown editors already do. Converting _from_ some other format _to_ Markdown may take more effort. In this case, I used a Google Doc add-on, [Docs to Markdown](https://workspace.google.com/marketplace/app/docs_to_markdown/700168918607).
2. Citation tool support. When writing in academia, I use an integrated tool for citation. [Zotero](https://www.zotero.org/), when installed as an add-on to Word or Google Docs, will help generate bibliographies and inline citations. I have managed to integrate Zotero integrations into my Markdown editor of choice ([Visual Studio Code](https://code.visualstudio.com/)), but it was _very_ fiddly. I followed the setup described in this video: [Setting Up a Scholarly Writing Environment With Markdown, VSCodium, and pandoc](https://youtu.be/J86Pm62XM_Q). Not for the faint of heart, with a very detailed how-to, step-by-step video, it still took me the better part of a Saturday, with reasonably in-depth knowledge of Markdown, Zotero, and my editor.

## Conclusion

To begin your Markdown journey, I suggest starting here: [Markdown Guide](https://www.markdownguide.org/). The easiest way to learn Markdown is to start using it; you can learn the basics in minutes. Once you do, you will find broad application and support. You can use Markdown to write HTML, [draft blog posts](https://wordpress.com/support/wordpress-editor/blocks/markdown-block/), create documentation, and post messages in messaging platforms or forums such as Reddit, Discord, and GitHub. 

[^1]: It seems worth mentioning, in a footnote, that I wrote this blog post entirely in Markdown. Feel free to download it and take a look. To see it with the formatted HTML, try pasting it in the online markdown editor [Dillinger](https://dillinger.io/).
