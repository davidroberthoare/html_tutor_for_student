# Lesson 4: CSS Introduction

## Learning Objectives

In this lesson, you will learn:
- What CSS is and why we use it
- How to link an external stylesheet
- Basic CSS syntax (selectors, properties, values)
- How to style text and backgrounds
- How to use element, class, and ID selectors

## Instructions

1. Open both `exercise.html` and `style.css` in VS Code
2. Link the stylesheet in your HTML head section
3. Add styles to make your page look better
4. Experiment with colors, fonts, and sizes
5. Preview your work using Live Server (changes show instantly!)

## What You're Building

A styled page about yourself with:
- Linked external stylesheet
- Custom colors for background and text
- Styled headings with different font sizes
- At least one class and one ID selector

## Success Criteria

Your page should:
- [ ] Link to style.css in the head section
- [ ] Display custom colors (not just browser defaults)
- [ ] Have styled headings (different colors or sizes)
- [ ] Use at least one class selector in CSS
- [ ] Use proper CSS syntax (selector { property: value; })
- [ ] Look visually different from an unstyled page

## Key Concepts to Remember

### Linking CSS
```html
<link rel="stylesheet" href="style.css">
```
This goes in the `<head>` section of your HTML.

### CSS Syntax
```css
selector {
  property: value;
  another-property: value;
}
```

### Types of Selectors
- `p` - Element selector (styles all p tags)
- `.classname` - Class selector (add class="classname" to HTML)
- `#idname` - ID selector (add id="idname" to HTML, use sparingly)

### Useful Properties
- `color` - text color
- `background-color` - background color
- `font-size` - text size (use px, like 18px)
- `font-family` - font choice

## Common Mistakes to Avoid

- Forgetting to link the stylesheet
- Wrong file path to CSS file
- Missing curly braces `{ }`
- Using `=` instead of `:` (it's `property: value`)
- Forgetting semicolons at end of each property
- Class selector without the dot (write `.myclass` not `myclass`)

## Getting Help

If styles aren't showing:
1. Check: Is style.css linked in HTML head?
2. Check: Is the filename exactly right?
3. Open browser DevTools (F12) → Console tab for errors
4. Ask Copilot: "My CSS isn't loading, what should I check?"

## Testing Your Work

1. Open in Live Server
2. Make a change in style.css and save
3. Page should update automatically
4. If colors aren't showing, check the console for errors
5. Right-click element → Inspect to see which styles are applied

## Experimentation Ideas

Try different values to see what happens:
- Change colors (use color names like 'navy', 'coral', 'teal')
- Try different font sizes (12px, 24px, 36px)
- Add background colors to different elements
- Style links to be a different color

## When You're Done

- Ask Copilot to "Check my work"
- Commit: `git add .` then `git commit -m "Complete Lesson 4 - CSS intro"`
- Want more? Ask: "Give me a challenge"

## Resources

- [MDN: CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
- [CSS Color Names](https://www.w3schools.com/colors/colors_names.asp)
- [Google Fonts](https://fonts.google.com/) - For custom fonts
