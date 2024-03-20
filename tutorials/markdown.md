# `Markdown`: Writing Content

```{note}
The content in this tutorial is from [Markdown CheatSheet](https://www.markdownguide.org/cheat-sheet/) by [Matt Cone](https://www.markdownguide.org/).
```

## Overview

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for basic syntax and extended syntax.

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

| Element | Markdown Syntax |
| --- | --- |
| Heading | `# H1`<br>`## H2`<br>`### H3` |
| Bold | `**bold text**` |
| Italic | `*italicized text*` |
| Blockquote | `> blockquote` |
| Ordered List | `1. First item`<br>`2. Second item`<br>`3. Third item` |
| Unordered List | `- First item`<br>`- Second item`<br>`- Third item` |
| Code | `` `code` `` |
| Horizontal Rule | `---` |
| Link | `[title](https://www.example.com)` |
| Image | `![alt text](image.jpg)` |

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

| Element | Markdown Syntax |
| --- | --- |
| Table | `\| Syntax \| Description \|`<br>`\| ----------- \| ----------- \|`<br>`\| Header \| Title \|`<br>`\| Paragraph \| Text \|` |
| Fenced Code Block | <pre>\```{<br>  "firstName": "John",<br>  "lastName": "Smith",<br>  "age": 25<br>}<br>\``` |
| Footnote | `Here's a sentence with a footnote. [^1]<br>[^1]: This is the footnote.` |
| Heading ID | `### My Great Heading {#custom-id}` |
| Definition List | <pre>Term 1<br>: Definition 1<br>Term 2<br>: Definition 2</pre> |
| Strikethrough | `~~The world is flat.~~` |
| Task List | `- [x] Write the press release`<br>`- [ ] Update the website`<br>`- [ ] Contact the media` |
| Emoji | `:smile:` |
| Highlight | `==highlighted==` |
| Subscript | `H~2~O` |
| Superscript | `4^th^` |

<!-- 
Whether you write your book's content in Jupyter Notebooks (`.ipynb`) or
in regular markdown files (`.md`), you'll write in the same flavor of markdown
called **MyST Markdown**.
This is a simple file to help you get started and show off some syntax.

## What is MyST?

MyST stands for "Markedly Structured Text". It
is a slight variation on a flavor of markdown called "CommonMark" markdown,
with small syntax extensions to allow you to write **roles** and **directives**
in the Sphinx ecosystem.

For more about MyST, see [the MyST Markdown Overview](https://jupyterbook.org/content/myst.html).

## Sample Roles and Directives

Roles and directives are two of the most powerful tools in Jupyter Book. They
are kind of like functions, but written in a markup language. They both
serve a similar purpose, but **roles are written in one line**, whereas
**directives span many lines**. They both accept different kinds of inputs,
and what they do with those inputs depends on the specific role or directive
that is being called.

Here is a "note" directive:

```{note}
Here is a note
```

It will be rendered in a special box when you build your book.

Here is an inline directive to refer to a document: {doc}`markdown-notebooks`.


## Citations

You can also cite references that are stored in a `bibtex` file. For example,
the following syntax: `` {cite}`holdgraf_evidence_2014` `` will render like
this: {cite}`holdgraf_evidence_2014`.

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

```{bibliography}
```

## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org). -->
