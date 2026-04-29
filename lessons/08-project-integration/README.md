# Lesson 8: Project Integration

## Learning Objectives

In this lesson, you will:
- Combine all skills learned (HTML structure, CSS styling, layout)
- Use semantic HTML for better structure
- Organize CSS effectively
- Follow best practices for code quality
- Create a complete, polished webpage
- Think about accessibility and user experience

## Instructions

1. Plan your project before coding (sketch it out!)
2. Create a complete webpage on a topic you're interested in
3. Use semantic HTML tags (header, nav, main, article, section, footer)
4. Write organized, commented CSS
5. Make it look polished and professional

## What You're Building

A complete webpage of your choice, such as:
- Personal portfolio or "about me" page
- Fan page for favorite book/movie/game/hobby
- Tutorial or how-to guide
- Information page about a topic you care about

## Success Criteria

Your project should:
- [ ] Use semantic HTML (header, main, section, article, footer, nav)
- [ ] Have logical heading hierarchy (h1 → h2 → h3)
- [ ] Include all content types: text, lists, links, images
- [ ] Have well-organized, commented CSS
- [ ] Use the box model effectively (margin, padding, border)
- [ ] Have a complete layout (header, main content, footer)
- [ ] Include meaningful alt text on all images
- [ ] Look polished and complete (not half-finished)
- [ ] Have good color contrast and readability
- [ ] Demonstrate understanding of all previous lessons

## Planning Your Project

**Before you code:**
1. **Choose your topic** - Something you're interested in!
2. **Sketch the layout** - Draw boxes on paper
3. **Plan the structure** - What sections do you need?
4. **Gather content** - Write text, collect images first
5. **Choose your style** - Pick colors and fonts

## Semantic HTML Reminder

Use meaningful tags:
```html
<header>      <!-- Site/page header -->
  <nav>       <!-- Navigation links -->
</nav>
</header>

<main>        <!-- Main content (one per page) -->
  <section>   <!-- Thematic grouping -->
    <article> <!-- Self-contained content -->
    </article>
  </section>
  
  <aside>     <!-- Related content, sidebar -->
  </aside>
</main>

<footer>      <!-- Site/page footer -->
</footer>
```

## CSS Organization

Organize your CSS with comments:
```css
/* === RESET/BASE === */
/* Global styles */

/* === LAYOUT === */
/* Header, main, footer structure */

/* === TYPOGRAPHY === */
/* Heading and text styles */

/* === COMPONENTS === */
/* Cards, buttons, navigation */

/* === UTILITIES === */
/* Helper classes */
```

## Code Quality Checklist

- [ ] Consistent indentation (2 or 4 spaces)
- [ ] Meaningful class names (.nav-link, not .x)
- [ ] Comments explaining major sections
- [ ] No inline styles (all CSS in external file)
- [ ] Consistent naming convention
- [ ] Grouped related code together
- [ ] Removed unused code

## Accessibility Checklist

- [ ] All images have alt text
- [ ] Good color contrast
- [ ] Logical heading hierarchy
- [ ] Descriptive link text
- [ ] Form labels (if you have forms)
- [ ] Semantic HTML structure

## Common Pitfalls to Avoid

- Starting to code before planning
- Using div for everything (use semantic tags!)
- Inconsistent styling
- Poor color contrast
- Missing alt text
- Skipping heading levels
- Unorganized CSS
- No comments in code

## Getting Help

This is an independent project, but Copilot can help:
- "I'm planning a page about [topic], what structure should I use?"
- "Is my layout approach good for [goal]?"
- "Check my HTML structure"
- "Is this accessible?"
- Ask questions about specific problems, not "build it for me"

## Testing Your Project

1. **Visual test**: Does it look complete and polished?
2. **Resize test**: Does it look okay at different widths?
3. **Link test**: Click every link—do they work?
4. **Image test**: Do all images load and have alt text?
5. **Code test**: Is it well-organized and commented?
6. **Accessibility test**: Is contrast good? Heading hierarchy logical?

## Taking It Further

Once your base project is done, consider:
- Adding hover effects with CSS transitions
- Making it responsive with media queries (research!)
- Adding smooth scrolling
- Using CSS animations
- Validating with W3C validator
- Testing with accessibility tools

## When You're Done

- Ask Copilot to "Check my work" (be ready to explain your code!)
- Commit: `git add .` then `git commit -m "Complete Lesson 8 - Full project"`
- **Celebrate!** You've completed the structured lessons!
- Move to the `projects/` folder for self-directed work
- Want more challenges? Ask: "Give me a challenge"

## What's Next?

After completing this lesson:
1. Move to the `projects/` folder
2. Build more complex projects independently
3. Explore new CSS properties and techniques
4. Keep learning and experimenting
5. Share your work with others!

## Resources

- [MDN: HTML Semantic Elements](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantic_elements)
- [W3C HTML Validator](https://validator.w3.org/)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [WebAIM: Web Accessibility](https://webaim.org/)

## Final Thoughts

You've learned the fundamentals of HTML and CSS! Everything else builds on this foundation. Keep practicing, keep building, and keep learning. Professional web developers are always learning new things too.

**You're now equipped to build any static website. The only limit is your creativity!**
