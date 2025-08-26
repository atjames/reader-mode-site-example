# Reader Mode Example - Lord of the Rings FAQ

A simple FAQ website about *The Lord of the Rings* that works perfectly in browser reader modes.

## What This Is

An example showing how to create a webpage that renders properly in browser reader mode. Uses Lord of the Rings FAQ content to demonstrate the HTML structure and techniques needed for reader mode compatibility.

## How to Write HTML for Reader Mode

Reader modes look for specific HTML patterns to extract content properly:

### Use Semantic HTML Elements
```html
<main>           <!-- Wrap your main content -->
  <h1>Title</h1> <!-- One main heading -->
  <section>      <!-- Group related content -->
    <h2>Question</h2>
    <p>Answer paragraph...</p>
  </section>
  <article>      <!-- Standalone content -->
    <h2>Article Title</h2>
    <p>Article content...</p>
    <blockquote>Quote text</blockquote>
  </article>
</main>
```

### Essential Elements
- `<main>` - Contains your primary content
- `<h1>` - One main title per page
- `<h2>` - Section headings (questions/articles)
- `<section>` - Groups related Q&A content
- `<article>` - Standalone pieces of content
- `<p>` - Body text paragraphs
- `<blockquote>` - Quoted text

### What Reader Mode Ignores
- Navigation menus
- Sidebars
- Ads and widgets
- Most CSS styling
- JavaScript content

### Things to Avoid (Will Break Reader Mode)
1. Using `<div>` instead of semantic elements for main content
2. Putting important content in JavaScript-generated elements
3. Using CSS to hide/show content instead of proper HTML structure
4. Complex nested layouts without clear content hierarchy
5. Missing or poorly structured heading tags (h1, h2, etc.)
6. Putting main content inside navigation or sidebar elements
