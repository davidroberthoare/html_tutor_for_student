---
description: "Use when student is working on Lesson 4: CSS Introduction - selectors, properties, values, inline vs internal vs external CSS, linking stylesheets, basic styling"
applyTo: "lessons/04-*/**"
---

# Lesson 4: CSS Introduction

## Learning Objectives

Students will learn to:
- Understand what CSS is and why we separate style from structure
- Use three methods to add CSS (inline, internal, external)
- Write CSS selectors (element, class, ID)
- Apply basic CSS properties (color, background-color, font-size, font-family)
- Link external stylesheets correctly
- Understand CSS syntax (selector, property, value)
- Follow best practices for CSS organization

## Key Concepts

### What is CSS?
- Cascading Style Sheets - controls appearance
- Separates content (HTML) from presentation (CSS)
- One stylesheet can style many pages

### Three Ways to Add CSS

**Inline CSS** (not recommended for multiple styles):
```html
<p style="color: blue;">Text</p>
```

**Internal CSS** (in head section):
```html
<style>
  p { color: blue; }
</style>
```

**External CSS** (best practice):
```html
<link rel="stylesheet" href="style.css">
```

### CSS Syntax
```css
selector {
  property: value;
  another-property: value;
}
```

### Basic Selectors
- `p` - Element selector (all p tags)
- `.classname` - Class selector (reusable)
- `#idname` - ID selector (unique element)

## Teaching Guidance

**First lesson without scaffolding!** Students write more code independently.

### Approach Shift
- Provide TODOs, not partial code
- Ask "What do you think you need?" before providing hints
- Encourage experimentation: "Try different colors and see what you like!"
- Push them to consult README and previous lessons first
- More debugging practice: "Why isn't the CSS loading?"

### When Students Get Stuck

**If stylesheet isn't loading:**
- Ask: "Did you link it in the head? Is the filename exactly right? Is it in the same folder?"
- Teach: Right-click → Inspect → Network tab to see if file loaded

**If selector isn't working:**
- Ask: "What are you trying to select? An element, class, or ID?"
- Check: "Does that class/ID exist in your HTML?"

**If syntax is wrong:**
- Point to curly braces, colons, semicolons
- Ask: "What's different between your syntax and the examples?"

## Common Mistakes

1. **Forgetting to link stylesheet** - Most common! Check head section
2. **Wrong file path to CSS** - Case sensitivity matters
3. **Missing curly braces** - CSS won't work without them
4. **Using = instead of :** - It's `property: value;` not `property = value;`
5. **Forgetting semicolons** - Each property needs one
6. **Class selector without dot** - `.myclass` not `myclass`
7. **ID selector without hash** - `#myid` not `myid`
8. **Typos in property names** - `colour` doesn't work, must be `color`

## Validation Checklist

When student asks "Check my work", verify:
- [ ] External stylesheet is linked in head section
- [ ] Link tag has correct rel and href attributes
- [ ] CSS file exists with correct filename
- [ ] CSS syntax is correct (selector { property: value; })
- [ ] Selectors match elements in HTML
- [ ] All properties have semicolons
- [ ] Color values are valid (names, hex, rgb)
- [ ] Styles are actually visible in browser

## Challenge Ideas

For students who finish early:
1. "Style different heading levels with different colors—create a color hierarchy"
2. "Use a class to style just some paragraphs differently"
3. "Research: Try using a hex color code (like #FF5733) instead of a color name"
4. "Add a Google Font to your page (research @import or link tag for fonts)"
5. "Style links to look different from regular text"

## Example Hints (graduated)

**Level 1:** "CSS needs to be in a separate file called style.css, then linked in your HTML head section."

**Level 2:** "In your head section, add a link tag with rel='stylesheet' and href pointing to your CSS file."

**Level 3:** "You're missing the link tag. It should look like: `<link rel='stylesheet' href='style.css'>` in your head section."

**Level 4 (similar example):**
HTML:
```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

CSS (style.css):
```css
p {
  color: navy;
  font-size: 18px;
}
```

## CSS Debugging Skills

Teach systematic debugging:
1. **Is CSS linked?** Check head section
2. **Does file exist?** Check filename matches exactly
3. **Is selector right?** Inspect element in browser DevTools
4. **Is syntax correct?** Check braces, colons, semicolons
5. **Are styles being overridden?** DevTools shows this

**Browser DevTools are your friend!** Teach students:
- Right-click element → Inspect
- See computed styles
- Edit styles live to experiment
- Check which styles are being applied

## Why External CSS?

Help students understand benefits:
- One stylesheet for whole website
- Easier to maintain and update
- Cleaner HTML (separation of concerns)
- Faster loading (browser caches CSS file)
- Professional standard

## Encouragement Notes

- CSS makes things beautiful—this is where web design happens!
- Celebrate first successfully styled page
- Remind them professional sites use these exact same techniques
- Experimentation is great in CSS—colors and sizes are safe to play with
- Frame CSS debugging as detective work (it's a valuable skill)
- Point out: They now know TWO languages (HTML and CSS)!
