# Reader Mode Example - Lord of the Rings FAQ

A simple FAQ website about *The Lord of the Rings* that works perfectly in browser reader modes.

## What This Is

A static FAQ site with questions and answers about Tolkien's Lord of the Rings. It's designed to be read by customers in browser reader mode for a distraction-free experience.

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
</main>
```

### Essential Elements
- `<main>` - Contains your primary content
- `<h1>` - One main title per page
- `<h2>` - Section headings (questions)
- `<section>` - Groups each Q&A pair
- `<p>` - Body text paragraphs

### What Reader Mode Ignores
- Navigation menus
- Sidebars
- Ads and widgets
- Most CSS styling
- JavaScript content

### Tips for Better Reader Mode
1. Use descriptive headings that make sense as questions
2. Keep paragraphs focused and not too long
3. Use `<em>` for emphasis instead of `<strong>` or `<b>`
4. Avoid complex layouts - simple is better
5. Test in Safari or Firefox reader mode to verify it works
