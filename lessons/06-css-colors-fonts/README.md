# Lesson 6: CSS Colors and Fonts

## Learning Objectives

In this lesson, you will learn:
- Different ways to specify colors (names, hex, rgb, rgba)
- How to choose and apply fonts
- How to use Google Fonts
- Text styling properties
- Creating visual hierarchy with typography
- Basic color theory for web design

## Instructions

1. Open `exercise.html` and `style.css`
2. Create a visually appealing page using colors and fonts
3. Import at least one Google Font
4. Create a consistent color scheme (3-5 colors)
5. Use typography to create clear hierarchy

## What You're Building

A beautifully styled page that demonstrates:
- Custom color scheme applied consistently
- Custom fonts from Google Fonts
- Text styling for readability
- Clear visual hierarchy

## Success Criteria

Your page should:
- [ ] Use at least 2 different color formats (hex, rgb, or named)
- [ ] Have a custom font from Google Fonts
- [ ] Show good contrast between text and background
- [ ] Use different font sizes to create hierarchy
- [ ] Have consistent color scheme (not random colors)
- [ ] Be readable and visually appealing

## Key Concepts to Remember

### Color Formats
```css
/* Named colors */
color: navy;

/* Hexadecimal */
color: #336699;  /* or shorthand: #369 */

/* RGB */
color: rgb(51, 102, 153);

/* RGBA (with transparency) */
color: rgba(51, 102, 153, 0.8);
```

### Font Properties
```css
font-family: Arial, Helvetica, sans-serif;  /* With fallbacks! */
font-size: 18px;
font-weight: bold;     /* or 100-900 */
font-style: italic;
line-height: 1.6;      /* Spacing between lines */
text-align: center;
text-decoration: underline;
letter-spacing: 1px;
```

### Using Google Fonts
1. Go to fonts.google.com
2. Select a font and styles
3. Copy the `<link>` into your HTML `<head>`
4. Use the font-family in your CSS

## Common Mistakes to Avoid

- Invalid hex codes (must be 3 or 6 digits after #)
- RGB values outside 0-255 range
- Font names without quotes when they have spaces
- No fallback fonts (always end with generic like sans-serif)
- Poor contrast (light text on light background)
- Too many different fonts (stick to 2-3)

## Design Tips

### Color Schemes
- Choose 3-5 colors that work well together
- Use a color palette generator (coolors.co)
- Ensure good contrast (dark text on light background or vice versa)
- Use accent colors sparingly

### Typography
- Body text: 16-18px minimum
- Line height: 1.4-1.8 for readability
- Limit line length: 50-75 characters
- Create hierarchy with size and weight

## Getting Help

Ask Copilot:
- "What color scheme would work well for [theme]?"
- "How do I add a Google Font?"
- "Is this color contrast good enough?"

## Testing Your Work

1. Zoom out—does hierarchy still work?
2. Squint test—can you still read it?
3. Check contrast with browser DevTools accessibility features
4. Ask someone else—is it readable?

## Challenge Yourself

Try:
- Creating a dark mode design
- Using RGBA for transparent backgrounds
- Text shadows for visual effects
- Multiple Google Font weights
- CSS variables for your color scheme

## When You're Done

- Ask Copilot to "Check my work"
- Commit: `git add .` then `git commit -m "Complete Lesson 6 - Colors and Fonts"`
- Want more? Ask: "Give me a challenge"

## Resources

- [Google Fonts](https://fonts.google.com/)
- [Coolors - Color Palette Generator](https://coolors.co/)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [MDN: Web Fonts](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts)
