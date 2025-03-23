---
title: "First post Tempore soluta velit reiciendis et omnis."
description: "Tempore soluta velit reiciendis et omnis. Ea illo voluptatibus dolor id rerum et. Et omnis asperiores nesciunt mollitia. Sunt sapiente vel laborum. Fugiat illo aliquam delectus culpa. Aliquam nobis consequatur architecto iure velit. Lorem ipsum dolor sit amet"
pubDate: "2025-01-01"
---

# Complete Markdown Test File for Astro + Tailwind Prose

This document contains examples of all markdown features supported by Astro and Tailwind's typography plugin (prose) to help test your implementation.

## Basic Typography

This is a paragraph with **bold text**, _italic text_, and **_bold italic text_**. You can also use **underscores** for bold and _underscores_ for italics.

This paragraph has `inline code` formatting.

Here's a [link to Astro's documentation](https://docs.astro.build) and an [internal link](#basic-typography).

Text can be ~~struck through~~ when needed.

## Headings

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

## Lists

### Unordered Lists

- Item 1
- Item 2
  - Nested item 2.1
  - Nested item 2.2
- Item 3

### Ordered Lists

1. First item
2. Second item
   1. Nested item 2.1
   2. Nested item 2.2
3. Third item

### Task Lists

- [x] Completed task
- [ ] Incomplete task
- [x] Another completed task

### Definition Lists

<dl>
  <dt>Astro</dt>
  <dd>A modern static site builder with server-side rendering capabilities.</dd>
  
  <dt>Tailwind</dt>
  <dd>A utility-first CSS framework for rapid UI development.</dd>
  
  <dt>Prose</dt>
  <dd>Tailwind's typography plugin that adds sensible styling to content from markdown or CMS.</dd>
</dl>

## Code Blocks

```javascript
// JavaScript code block
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet("Astro Developer"));
```

```css
/* CSS code block */
.prose h1 {
  font-weight: 800;
  margin-top: 2em;
}

.prose pre {
  background-color: #1e293b;
  color: #e2e8f0;
}
```

```jsx
// JSX/React component
import React from "react";

const Greeting = ({ name }) => {
  return (
    <div className="prose">
      <h1>Hello, {name}!</h1>
      <p>Welcome to your Astro + Tailwind blog.</p>
    </div>
  );
};

export default Greeting;
```

## Blockquotes

> This is a blockquote.
>
> It can span multiple paragraphs.
>
> > And can be nested.

## Tables

| Feature     | Astro Support | Tailwind Prose |
| ----------- | ------------- | -------------- |
| Headings    | ✅            | ✅             |
| Lists       | ✅            | ✅             |
| Code blocks | ✅            | ✅             |
| Images      | ✅            | ✅             |
| Tables      | ✅            | ✅             |

## Horizontal Rule

---

## Images

![Astro Logo](https://astro.build/assets/press/astro-logo-dark.svg)

## HTML Elements

Astro and Tailwind Prose can handle HTML elements directly in markdown:

<div class="custom-container">
  <p>This is a custom container with HTML.</p>
  <button class="btn">Click me</button>
</div>

<details>
  <summary>Click to expand</summary>
  <p>This is hidden content that can be expanded.</p>
</details>

## Footnotes

Here's a sentence with a footnote[^1].

[^1]: This is the footnote content.

## Subscript and Superscript

H<sub>2</sub>O is water and 2<sup>10</sup> is 1024.

## Highlighting

==This text is highlighted== (Note: This may require additional plugins)

## Front Matter (for Astro)

Note that your actual Astro markdown files should include frontmatter at the top, like this:

```yaml
---
title: Complete Markdown Test
description: Testing all Markdown features in Astro with Tailwind Prose
publishDate: 2025-03-22
author: Your Name
image:
  url: /images/blog-post-image.jpg
  alt: Blog post featured image
tags:
  - astro
  - tailwind
  - markdown
  - tutorial
---
```

## Math Expressions (with KaTeX or MathJax plugin)

If you've added KaTeX or MathJax support, test it with:

$$
f(x) = \int_{-\infty}^{\infty} \hat{f}(\xi) e^{2\pi i \xi x} d\xi
$$

Inline math: $E = mc^2$

## Astro-specific features

Astro allows you to include components directly in your markdown with MDX. If you're using MDX, you could test it with:

```astro
import Button from '../components/Button.astro'; # My MDX Page with Components

<Button text="Click me!" />
```

## Tailwind Prose Classes Test

Tailwind Prose adds styling to many elements. Here are some to test:

- Long paragraphs should have good line height and spacing: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam euismod, nisl eget aliquam ultricies, nunc nisl aliquet nunc, eget aliquam nisl nunc vel nisl. Nullam euismod, nisl eget aliquam ultricies, nunc nisl aliquet nunc, eget aliquam nisl nunc vel nisl.

- `prose-sm`, `prose-base`, `prose-lg`, `prose-xl`, and `prose-2xl` classes can be tested by adding them to your container.

- The `prose-invert` class can be used for dark mode.

- The `prose-red`, `prose-yellow`, `prose-green`, etc. classes can be used to change the theme color.

## Interactive Elements

Astro supports interactive elements through islands architecture. If you have client-side JavaScript, you may have things like:

<div class="interactive-demo" data-astro-reload>
  <p>This would be an interactive component in a real implementation.</p>
</div>

## Embedding Content

Astro supports embedding content from other sources:

<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

This is the end of the test file. If all of the above renders correctly, your Astro + Tailwind Prose implementation is working properly.
