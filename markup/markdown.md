# Markup / Markdown

Markdown is the most common markup language I have seen. It is supported by many coding environments, and has a multitude of flavors.

## Spacing

All block elements need a line in-between. This helps organize. No more than this, though.

```markdown
# Heading

See there is a space in-between ^

> Some more text

## Subheading

Even through headings, there is still only a single line.
```

## Titles

The start of a markdown document contains a Heading 1 (`<h1>`). This specifies the title. This heading will never be used again in the document. All sections will be Heading 2s, sub-sections H3s, and so-on.

## Paragraphs

Line width usually does not matter, as soft-wrapping is a common feature in IDEs. A markdown writer should not feel the need to add newlines, unless they wish to.

```markdown
> You can add a newline in-between sentences, though it is unecessary and won't render.

This is the third line.
This is the fourth line.
```

```html
<!-- Output -->
<blockquote>You can add a newline in-between sentences, though it is unecessary and won't render.</blockquote>
<p>This is the third line. This is the fourth line.</p>
```

## Specifying Author

To specify the author of the article, put a blockquote directly below the title.

> This is a blockquote

```markdown
# Title of Article

> Written by: BD103
```

## Code Blocks

When writing code in your markup, always try to specify the language. This is by writing the language name directly next to the three backticks (\`\`\`) at the start of the code block. If there is no language, don't write one.

It is hard to give examples for code blocks, so feel free to inspect this raw document!

## Inline Formatting

When giving inline formatting (eg. with asterisks or underscores), pretend that they work the same as parenthese. Don't put a space between them and the word.

```markdown
# Good example

These are some _inline_ italics.

# Bad example

These are some _ inline _ italics.
```