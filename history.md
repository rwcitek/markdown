# Why Markdown?  The Pre-Markdown Era: A History of Lightweight Markup

Before John Gruber and Aaron Swartz designed Markdown in 2004 to bridge the gap between 
human-readable plain text and web-ready HTML, a rich ecosystem of specialized markup 
languages already existed. 
These ancestral and parallel formats were developed to solve specific problems: 
documenting software, powering collaborative wikis, and standardizing multi-format technical publishing.

## 1986: GNU Texinfo

### The Purpose: Multi-Format Technical Documentation

Long before the World Wide Web, the GNU Project needed a way to write software manuals that could be read both on a computer screen (via terminal menus) and printed as high-quality physical books. Created by **Richard Stallman** in 1986, **Texinfo** became the official documentation format for the GNU Project.

Texinfo uses a syntax prefixed with the `@` character (highly influenced by an earlier system called Scribe). A single Texinfo source file can be compiled into:

* **Info files:** A text-based, interactive hypertext system read in the terminal using the `info` command.
* **TeX / PDF:** Beautifully typeset physical or digital books.
* **HTML:** Modern web pages (added later as the web evolved).

While incredibly powerful for massive technical manuals, Texinfo is not "lightweight" by modern standards; its strict macros and structural commands make it closer to LaTeX or HTML than plain text.

```texinfo
@node Top
@chapter Introduction to Example Program

This is a sample paragraph in a Texinfo file.

@itemize @bullet
@item
First point with a @code{code_sample}.
@item
Second point.
@end itemize

```

## 1994: POD (Plain Old Documentation) & perldoc

### The Purpose: Embedding Readable Docs in Source Code

In 1994, Larry Wall introduced **POD (Plain Old Documentation)** with Perl 5. POD was born out of a desire to keep software documentation strictly intertwined with the source code itself, ensuring that developers wouldn't forget to update the manual when they updated the code.

The defining trait of POD is its extreme simplicity and readability in raw form. The Perl compiler is built to completely ignore POD blocks, while the **`perldoc`** command-line tool parses them to display clean, formatted man-pages directly in the terminal.

Key features of POD include:

* **Paragraph-based parsing:** Blank lines separate blocks.
* **Command paragraphs:** Start with an `=` sign (e.g., `=head1`, `=item`).
* **Verbatim paragraphs:** Indented text is automatically treated as literal code blocks.
* **Interior sequences:** Simple formatting codes like `B<bold>` or `I<italic>`.

```pod
=head1 NAME

Module::Example - A simple POD demonstration

=head2 SYNOPSIS

    use Module::Example;
    my $obj = Module::Example->new();

=head1 DESCRIPTION

This is an ordinary paragraph explaining the module. You can make 
text B<bold> or I<italic> easily.

=cut

```

## 1995: Wikitext (Wiki Markup)

### The Purpose: Rapid, Collaborative Web Editing

When Ward Cunningham created the first-ever wiki (WikiWikiWeb) in 1995, 
he needed a way for everyday users to write and link web pages instantly without 
forcing them to write raw, dangerous, or tedious HTML. This gave birth to **Wikitext** (or Wiki markup).

Unlike Texinfo and POD—which were built for software and technical documentation—Wikitext was built purely for the open web. 
It democratized content creation by using intuitive keyboard symbols to mimic visual styling:

* Putting text in single quotes `''italic''` or `'''bold'''` for emphasis.
* Using asterisks `*` for lists.
* Using square brackets `[[Page Name]]` to instantly create hyperlinks to other pages.

Wikitext would later be scaled to global prominence by Wikipedia using the MediaWiki engine. 
However, because early wiki engines were highly localized, hundreds of different "wikitext dialects" 
emerged, making it difficult to move text from one wiki to another.

```wikitext
== Introduction ==
Welcome to the wiki. You can read about the [[History of Computing]].

* '''Bold item'''
* ''Italic item''

```

[Example of wikitext of the Markdown page]( https://en.wikipedia.org/w/index.php?title=Markdown&action=edit )


## The Road to Markdown (2004)

By the early 2000s, internet users had seen various approaches to formatting text without raw HTML:

1. **Texinfo** proved that multi-output documentation from a single source file was viable.
2. **POD** proved that formatting syntax could be entirely non-intrusive and readable as plain text.
3. **Wikitext** proved that simplified punctuation rules could power massive web platforms.

However, Wikitext was often messy, and POD was explicitly tethered to programming. 
John Gruber sought to extract the absolute best elements of these formats—alongside the conventions people already used
instinctively in text-only emails (like adding a `>` for blockquotes or `#` for emphasis)—to create **Markdown**: 
a universally applicable, maximally human-readable format optimized specifically for web writers.


## 2004: The Creation
Markdown was created in **2004** by **John Gruber** in collaboration with **Aaron Swartz**. 
Gruber's goal was to enable people "to write using an easy-to-read, easy-to-write plain text format, 
then convert it to structurally valid XHTML (or HTML)."

The key design philosophy was **readability**:
> "A Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions."

## Evolution and the Fragmentation Era
As Markdown grew in popularity, developers started using it for various platforms (like GitHub, Reddit, and Stack Overflow).
However, Gruber’s original syntax description left many edge cases undefined. 
This led to different implementations creating their own custom behaviors, features, and flavors.

Some popular "flavors" emerged:
* **GitHub Flavored Markdown (GFM):** Added tables, task lists, and autolinking.
* **Markdown Extra:** Added support for footnotes and definition lists.
* **MultiMarkdown:** Expanded formatting features for advanced publishing.

## 2014: CommonMark
To address the fragmentation and lack of a formal specification, a group of developers launched an effort in 2014 to standardize Markdown. 
This resulted in **CommonMark**, a highly specified version of Markdown with a strict grammar and comprehensive test suite 
to ensure consistent rendering across different platforms.

## Present Day
Today, Markdown is the undisputed standard for:
1.  Software documentation (`README.md` files)
2.  Static site generators (Jekyll, Hugo, Astro)
3.  Note-taking applications (Obsidian, Notion)
4.  Technical blogging and communication

It remains one of the most widely adopted tools for digital writing due to its simplicity, speed, and platform-independence.



