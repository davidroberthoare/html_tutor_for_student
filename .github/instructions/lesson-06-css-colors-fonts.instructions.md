---
description: "Use when student is working on Lesson 6: CSS Colors and Fonts - color systems (names, hex, rgb), font properties, font-family, web fonts, text styling"
applyTo: "lessons/06-*/**"
---

# Lesson 6: CSS Colors and Fonts

## Learning Objectives

Students will learn to:
- Use different color value formats (names, hex, rgb, rgba)
- Apply color to text and backgrounds
- Understand font properties (family, size, weight, style)
- Use web-safe fonts and font stacks
- Import and use custom fonts (Google Fonts)
- Style text with various properties
- Create visual hierarchy with typography
- Understand web font loading

## Key Concepts

### Color Values

**Named Colors**:
```css
color: blue;
background-color: lightgray;
```

**Hexadecimal** (most common):
```css
color: #FF5733;  /* #RRGGBB */
color: #F73;     /* Shorthand for #FF7733 */
```

**RGB and RGBA**:
```css
color: rgb(255, 87, 51);          /* Red, Green, Blue */
color: rgba(255, 87, 51, 0.5);    /* With alpha (transparency) */
```

### Font Properties

**Font Family** (with fallback stack):
```css
font-family: Arial, Helvetica, sans-serif;
font-family: 'Times New Roman', Times, serif;
```

**Other Font Properties**:
```css
font-size: 18px;           /* Size */
font-weight: bold;         /* Weight: normal, bold, or 100-900 */
font-style: italic;        /* Style: normal or italic */
line-height: 1.6;          /* Spacing between lines */
```

**Text Properties**:
```css
text-align: center;        /* left, center, right, justify */
text-decoration: underline;/* underline, line-through, none */
text-transform: uppercase; /* uppercase, lowercase, capitalize */
letter-spacing: 2px;       /* Space between letters */
```

### Web Fonts (Google Fonts)

In HTML head:
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

In CSS:
```css
font-family: 'Roboto', sans-serif;
```

## Teaching Guidance

**Emphasize creativity!** This lesson is fun—colors and fonts bring personality to pages.

### Approach
- Encourage experimentation with colors and fonts
- Let students explore and develop their own aesthetic
- Teach color theory basics (contrast, readability)
- Discuss accessibility (readable text, sufficient contrast)
- Push them to create cohesive color schemes

### When Students Get Stuck

**If colors don't look right:**
- Ask: "What feeling are you trying to create?"
- Teach: Use color picker tools or palette generators
- Discuss: Contrast matters for readability

**If fonts aren't loading:**
- Ask: "Did you link the Google Font in your head section?"
- Check: Is the font name spelled exactly right in CSS (including capitals)?
- Teach: Font names with spaces need quotes

**If text is hard to read:**
- Ask: "Is there enough contrast between text and background?"
- Teach: Test readability by squinting or zooming out

## Common Mistakes

1. **Invalid hex codes** - Must be 3 or 6 characters after #
2. **Missing # in hex colors** - Won't work without it
3. **RGB values out of range** - Must be 0-255
4. **Font names without quotes** - Multi-word fonts need quotes: `'Times New Roman'`
5. **No fallback fonts** - Always provide font stack in case first font fails
6. **Poor contrast** - Light text on light background is unreadable
7. **Too many different fonts** - Usually stick to 2-3 font families max
8. **Forgetting to import web fonts** - Font won't load if link is missing
9. **Generic font family at start** - Should be at end: `Arial, sans-serif` not `sans-serif, Arial`

## Validation Checklist

When student asks "Check my work", verify:
- [ ] Color values are valid (named, hex with #, or correct rgb)
- [ ] Text has sufficient contrast with background
- [ ] Font-family has fallback stack (ends with generic like sans-serif)
- [ ] Web fonts are properly linked in head
- [ ] Font sizes are readable (not too small)
- [ ] Line height makes text readable (1.4-1.8 usually good)
- [ ] Not too many different fonts (2-3 max recommended)
- [ ] Text styling enhances readability, not hinders it
- [ ] Can explain their color and font choices

## Challenge Ideas

For students who finish early:
1. "Create a color scheme with a primary, secondary, and accent color. Use them consistently throughout your page"
2. "Use Google Fonts to find and implement a custom font that matches your page's personality"
3. "Create a dark mode color scheme with light text on dark backgrounds"
4. "Research: Use CSS variables to store your colors for easy reuse"
5. "Experiment with font-weight values (100-900) if using a Google Font with multiple weights"
6. "Create a text gradient using background-clip (advanced, requires research)"
7. "Use rgba to create semi-transparent backgrounds"

## Example Hints (graduated)

**Level 1:** "Colors can be written as names (blue), hex codes (#0000FF), or rgb values rgb(0, 0, 255). Try different formats!"

**Level 2:** "Your hex code is missing the # symbol. Hex colors need to start with #, like #FF5733"

**Level 3:** "For that custom font to work, you need to: 1) link it in HTML head from Google Fonts, 2) use it in your CSS with the exact name in quotes"

**Level 4 (similar example):**
HTML:
```html
<head>
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">
</head>
```

CSS:
```css
body {
  font-family: 'Open Sans', Arial, sans-serif;
  color: #333;
  background-color: #f5f5f5;
}

h1 {
  color: #2c3e50;
  font-size: 36px;
}
```

## Design Teaching Points

**Color Theory Basics:**
- **Contrast**: Dark text on light background or vice versa
- **Harmony**: Colors that work well together
- **Accent colors**: Use sparingly for emphasis
- **Consistency**: Stick to a palette (3-5 colors)

**Typography Tips:**
- **Hierarchy**: Headings larger than body text
- **Readability**: 16px minimum for body text
- **Line height**: 1.4-1.8 for body text (more space = easier to read)
- **Line length**: 50-75 characters per line is ideal
- **Font pairing**: Contrast heading and body fonts (e.g., serif + sans-serif)

**Accessibility:**
- Text and background need 4.5:1 contrast ratio minimum
- Don't rely only on color to convey information
- Test readability by zooming or using contrast checker tools

## Finding and Using Google Fonts

Walk students through the process:
1. Go to fonts.google.com
2. Browse and select a font
3. Click "Select this style" for weights you want
4. Copy the `<link>` tag into HTML head
5. Copy the CSS `font-family` declaration
6. Always add fallback fonts after the custom font

## Color Resources

Suggest helpful tools:
- Color palettes: coolors.co
- Contrast checker: webaim.org/resources/contrastchecker
- Color names: htmlcolorcodes.com
- Inspiration: dribbble.com, behance.net (show real designs)

## Encouragement Notes

- This is where personal style emerges—celebrate creative choices!
- Good typography is the foundation of web design
- Remind them that consistent use of colors and fonts looks professional
- Point out that they're making real design decisions
- Frame "mistakes" as experiments that teach you what doesn't work
- Celebrate when they explain their design rationale ("I chose blue because...")
- This is often students' favorite lesson—let them have fun!
