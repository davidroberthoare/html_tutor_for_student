---
description: "Use when student is working on Lesson 8: Project Integration - combining all skills, semantic HTML, best practices, building complete pages, accessibility basics"
applyTo: "lessons/08-*/**"
---

# Lesson 8: Project Integration

## Learning Objectives

Students will learn to:
- Combine all learned HTML and CSS skills in a complete project
- Write semantic HTML for better structure and accessibility
- Organize CSS effectively
- Follow best practices for code quality
- Understand basic accessibility principles
- Debug complex multi-file projects
- Create a polished, complete webpage
- Think about user experience

## Key Concepts

### Semantic HTML

Use meaningful tags that describe content:

**Good semantic HTML:**
```html
<header>
  <nav>...</nav>
</header>
<main>
  <article>
    <h1>...</h1>
    <p>...</p>
  </article>
  <aside>...</aside>
</main>
<footer>...</footer>
```

**Not semantic** (but still works):
```html
<div>
  <div>...</div>
</div>
<div>
  <div>
    <div>...</div>
    <div>...</div>
  </div>
</div>
<div>...</div>
```

### Semantic Tags

- `<header>` - Site/section header
- `<nav>` - Navigation links
- `<main>` - Main content (one per page)
- `<article>` - Self-contained content (blog post, card)
- `<section>` - Thematic grouping
- `<aside>` - Tangentially related content (sidebar)
- `<footer>` - Site/section footer
- `<figure>` and `<figcaption>` - Images with captions

### CSS Organization

**Good practices:**
1. Group related styles together
2. Use comments to separate sections
3. Order: layout → typography → colors → details
4. Consistent naming conventions
5. Avoid redundancy (use classes for repeated styles)

```css
/* === LAYOUT === */
.container { ... }

/* === TYPOGRAPHY === */
body { font-family: ...; }

/* === COMPONENTS === */
.card { ... }

/* === UTILITIES === */
.text-center { ... }
```

### Accessibility Basics

- Alt text on all images
- Semantic HTML for structure
- Sufficient color contrast
- Descriptive link text (not "click here")
- Logical heading hierarchy
- Form labels (future lesson)

## Teaching Guidance

**Capstone lesson!** Students integrate everything they've learned.

### Approach
- Students work on a complete project with minimal scaffolding
- Ask high-level questions: "What's your plan?" "How will you structure this?"
- Encourage planning before coding
- Push for thoughtful decisions: "Why did you choose that structure?"
- Celebrate their independence and problem-solving

### When Students Get Stuck

**If overwhelmed:**
- Ask: "What's the first small thing you could build?"
- Teach: Break big projects into small tasks
- Suggest: Start with HTML structure, then basic CSS, then refinement

**If structure is unclear:**
- Ask: "What are the main sections of your page?"
- Sketch: Draw boxes to visualize layout before coding
- Think: "If this were a newspaper, what would be header, articles, sidebar?"

**If code is messy:**
- Ask: "If you came back to this in a month, could you understand it?"
- Teach: Good code is readable code
- Suggest: Add comments, organize sections, use consistent naming

## Common Mistakes

1. **Using div for everything** - Use semantic tags when appropriate
2. **Inconsistent naming** - Pick a style (camelCase, kebab-case) and stick to it
3. **No code organization** - Random order makes maintenance hard
4. **Missing alt text** - Every img needs alt, even if empty (`alt=""` for decorative)
5. **Poor heading hierarchy** - Don't skip heading levels
6. **Inline styles** - Should use external CSS by now
7. **No planning** - Jumping into code without thinking about structure
8. **Repetitive CSS** - Could use classes instead of repeating styles

## Validation Checklist

When student asks "Check my work", verify:
- [ ] Uses semantic HTML where appropriate
- [ ] Logical document structure (header, main, footer)
- [ ] All images have alt text
- [ ] Heading hierarchy makes sense (h1 → h2 → h3, no skipping)
- [ ] CSS is organized with comments
- [ ] Consistent naming conventions
- [ ] Code is readable and indented properly
- [ ] No inline styles (all CSS in external file)
- [ ] Colors have sufficient contrast
- [ ] Links have descriptive text
- [ ] Page looks complete and polished
- [ ] Can explain their structural and design decisions

## Challenge Ideas

For students who finish early:
1. "Add a 'skip to main content' link for accessibility (research: skip links)"
2. "Make your layout responsive with media queries (research topic)"
3. "Add smooth scrolling behavior to anchor links"
4. "Create a print stylesheet so your page looks good when printed"
5. "Validate your HTML and CSS using W3C validators"
6. "Test your page with a screen reader or browser's accessibility tools"
7. "Add CSS transitions for hover effects"
8. "Optimize your images for web (research image optimization)"

## Example Hints (graduated)

**Level 1:** "Think about the major sections of your page. Header? Main content? Footer? Start by creating that structure with semantic tags."

**Level 2:** "Instead of using div for your navigation, use the `<nav>` tag. For your page header, use `<header>`. This makes your structure more meaningful."

**Level 3:** "Your page structure could be: `<header>` with `<nav>` inside, `<main>` with your content, then `<footer>`. Replace some of your divs with these semantic tags."

**Level 4 (similar example):**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <nav>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
    </nav>
  </header>
  
  <main>
    <section id="about">
      <h1>About Me</h1>
      <p>...</p>
    </section>
    
    <section id="projects">
      <h2>My Projects</h2>
      <article class="project">
        <h3>Project 1</h3>
        <p>...</p>
      </article>
    </section>
  </main>
  
  <footer>
    <p>&copy; 2026 My Name</p>
  </footer>
</body>
</html>
```

## Project Planning Process

Teach students to plan before coding:

1. **Sketch**: Draw boxes on paper for layout
2. **Structure**: List the HTML sections you'll need
3. **Content**: Gather text, images before starting
4. **Build**: HTML first (structure), then CSS (style)
5. **Refine**: Test, debug, improve
6. **Review**: Read your code like someone else wrote it

## Code Quality Teaching

**Readability matters:**
- Consistent indentation (2 or 4 spaces)
- Meaningful class names (`.nav-link` not `.x`)
- Comments for major sections
- Grouped related code
- Whitespace for visual separation

**Good code is:**
- Easy to understand
- Easy to modify
- Well-organized
- Consistent in style

## Semantic HTML Benefits

Help students understand why semantic tags matter:
- **SEO**: Search engines understand content better
- **Accessibility**: Screen readers can navigate by landmarks
- **Readability**: Other developers understand your structure
- **Maintainability**: Clear structure is easier to update
- **Future-proof**: Works better with new technologies

## Real-World Context

This is the culmination of their learning:
- They can now build real web pages
- They know the same tools professionals use
- They understand both structure (HTML) and style (CSS)
- They can learn any new web technology (React, etc.) because they know the foundation

## Encouragement Notes

- Celebrate completing the structured lessons!
- Emphasize how far they've come from Lesson 1
- Point out: They can now build ANY static website
- Frame this as a beginning, not an end
- Encourage them to keep building and learning
- Remind them: Professional developers are always learning too
- Celebrate their problem-solving growth throughout the course
- Point out: They now know how to work effectively with AI for learning
- They've learned two skills: web development AND how to learn with AI
- The real project work begins now—encourage creativity!

## After This Lesson

Students should move to the `projects/` folder where they can:
- Build personal pages
- Create hobby sites
- Experiment with creative designs
- Combine everything they've learned
- Work on self-directed learning
- Explore new CSS properties and techniques
- Start preparing portfolios

The training wheels are off—time to build!
