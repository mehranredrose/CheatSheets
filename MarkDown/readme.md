# Markdown Cheat Sheet

Markdown is a lightweight markup language that allows you to format text easily using plain text editor. It is often used for writing emails, readme files, and documentation. Below is a detailed cheat sheet to help you get started with Markdown.

## Basics

### Headings
Headings are defined by one or more `#` symbols at the beginning of the line, followed by a space.

```markdown
# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading
```

### Paragraphs and Line Breaks
Paragraphs are simply blocks of text separated by one or more blank lines. To create a line break within a paragraph, use two spaces at the end of the line.

```markdown
This is a paragraph.  
And this is another line in the same paragraph.
```

## Styling Text

### Bold and Italic
You can make text bold using `**` or `__`, and italic using `*` or `_`.

```markdown
**Bold text**
__Bold text__
*Italic text*
_Italic text_
```

### Strikethrough
Use two tildes (`~~`) to strike through text.

```markdown
~~Strikethrough~~
```

## Links

Links are created using the following syntax:

```markdown
[Link Text](URL)
```

Example:

```markdown
[Markdown Guide](https://www.markdownguide.org/)
```

### Email Links
Email links can also be created:

```markdown
<example@example.com>
```

## Images

Images are similar to links, but they include an alt text.

```markdown
![Alt Text](URL)
```

Example:

```markdown
![Markdown Logo](https://markdown-here.com/img/icon256.png)
```

## Lists

### Unordered List
Unordered lists start with `-`, `+`, or `*`.

```markdown
- Item 1
- Item 2
- Item 3
```

Example:

```markdown
- Apple
- Banana
- Cherry
```

### Ordered List
Ordered lists start with numbers followed by a period.

```markdown
1. First step
2. Second step
3. Third step
```

Example:

```markdown
1. Go to the store.
2. Buy bread.
3. Return home.
```

## Blockquotes

Blockquotes are created using `>`.

```markdown
> This is a blockquote.
> It can span multiple lines.
```

Example:

```markdown
> Markdown is a lightweight markup language.
> It is often used for writing emails, readme files, and documentation.
```

## Code

### Inline Code
Use backticks (`` ` ``) to highlight inline code.

```markdown
`print("Hello, World!")`
```

Example:

```markdown
In Python, you can use the `print()` function to output text.
```

### Code Blocks
Code blocks are created by indenting the code four spaces or enclosing it in triple backticks (```).

#### JavaScript
```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}
```

#### HTML
```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page</title>
</head>
<body>
  <h1>Hello, World!</h1>
</body>
</html>
```

#### CSS
```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}
```

## Horizontal Rule

Horizontal rules are created using three or more dashes (`---`), asterisks (`***`), or underscores (`___`).

```markdown
---
***
___
```

Example:

```markdown
This is a paragraph.

---

This is another paragraph.
```

## Tables

Tables can be created using pipes (|) and hyphens (-).

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1, Cell 1 | Row 1, Cell 2 | Row 1, Cell 3 |
| Row 2, Cell 1 | Row 2, Cell 2 | Row 2, Cell 3 |
```

Example:

```markdown
| First Name | Last Name | Age |
|------------|-----------|-----|
| John       | Doe       | 30  |
| Jane       | Smith     | 25  |
```

## Footnotes

Footnotes are created using `[^1]` in the text and `[^1]: Footnote Content` at the bottom of the document.

```markdown
This is a sentence with a footnote[^1].

[^1]: This is the footnote content.
```

Example:

```markdown
Markdown supports footnotes[^1].

[^1]: This is the footnote content.
```

## Emoji

You can use emojis by typing `:` followed by the emoji name and ending with another `:`. You can find a list of available emojis [here](https://www.webfx.com/tools/emoji-cheat-sheet/).

```markdown
This sentence has an :smile:
```

Example:

```markdown
I'm feeling :happy:. This is great!
```

## Task Lists

Task lists are similar to ordered lists but include checkboxes.

```markdown
- [ ] Task 1
- [x] Task 2
- [ ] Task 3
```

Example:

```markdown
- [ ] Prepare the presentation
- [x] Schedule the meeting
- [ ] Review the budget
```

This cheat sheet provides a comprehensive overview of Markdown syntax. By mastering these elements, you can effectively format your text for clarity and readability.

Happy writing!
```

You can save this content in a file named `markdown.md` in your cheatsheets directory. Feel free to modify it further to suit your needs!
