# Lesson 7: Layout Basics

## Learning Objectives

In this lesson, you will learn:
- The display property (block, inline, inline-block)
- Positioning (static, relative, absolute, fixed)
- Flexbox fundamentals for layouts
- How to center elements
- Creating common layout patterns
- Using browser DevTools to debug layouts

## Instructions

1. Open `exercise.html` and `style.css`
2. Create a page with a header, main content, and footer
3. Use flexbox to create layouts
4. Experiment with positioning
5. Build at least one navigation bar using flexbox

## What You're Building

A complete page layout with:
- Header with navigation (using flexbox)
- Main content area
- Sidebar (optional challenge)
- Footer
- Proper use of display and positioning

## Success Criteria

Your page should:
- [ ] Have a navigation bar using flexbox
- [ ] Use display: flex at least twice
- [ ] Center at least one element
- [ ] Show understanding of flex container vs flex items
- [ ] Have a clear layout structure
- [ ] Demonstrate at least one use of positioning

## Key Concepts to Remember

### Display Property
```css
display: block;         /* Takes full width, stacks vertically */
display: inline;        /* Flows horizontally, no width/height */
display: inline-block;  /* Flows horizontally, respects width/height */
display: flex;          /* Flexbox container */
```

### Positioning
```css
position: static;       /* Default, normal flow */
position: relative;     /* Offset from normal position */
position: absolute;     /* Positioned relative to parent */
position: fixed;        /* Fixed to viewport */

/* With relative, absolute, or fixed: */
top: 10px;
right: 20px;
bottom: 10px;
left: 20px;
```

### Flexbox Basics
```css
/* Container (parent) */
.container {
  display: flex;
  justify-content: center;    /* Horizontal alignment */
  align-items: center;        /* Vertical alignment */
  flex-direction: row;        /* or column */
  gap: 20px;                  /* Space between items */
}

/* Items (children) */
.item {
  flex: 1;                    /* Grow to fill space */
}
```

## Common Mistakes to Avoid

- Forgetting `display: flex` on the container
- Putting flexbox properties on wrong elements
- Absolute positioning without a positioned parent
- Using positioning for everything (margin is often simpler!)
- Inline elements with width/height (won't work)

## Layout Patterns to Try

### Navigation Bar
```css
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

### Centered Content
```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 300px;
}
```

### Three Columns
```css
.columns {
  display: flex;
  gap: 20px;
}
.column {
  flex: 1;
}
```

## Using DevTools to Debug

1. Right-click element → Inspect
2. Toggle flex properties on/off to see effects
3. Check if `display: flex` is applied
4. Visualize flex directions and spacing
5. Test different justify-content values live

## Getting Help

Ask Copilot:
- "How do I center this element?"
- "My flexbox isn't working, what should I check?"
- "Should I use flexbox or positioning for [layout]?"

## Testing Your Work

1. Resize browser window—does layout adapt?
2. Check navigation bar—are items spaced properly?
3. Use DevTools to inspect flex containers
4. Verify positioning works as expected
5. Make sure nothing overlaps unintentionally

## Challenge Yourself

Try creating:
- A sticky navigation bar (stays at top when scrolling)
- A three-column layout
- A centered card using flexbox
- A footer that always stays at bottom
- A responsive image gallery

## When You're Done

- Ask Copilot to "Check my work"
- Commit: `git add .` then `git commit -m "Complete Lesson 7 - Layouts"`
- Want more? Ask: "Give me a challenge"

## Resources

- [MDN: Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
- [Flexbox Froggy](https://flexboxfroggy.com/) - Interactive game to learn flexbox
- [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN: Positioning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)
