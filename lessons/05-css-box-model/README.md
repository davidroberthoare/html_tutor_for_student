# Lesson 5: CSS Box Model

## Learning Objectives

In this lesson, you will learn:
- Understanding the box model (content, padding, border, margin)
- The difference between margin and padding
- How to add borders to elements
- How to control element dimensions
- How to use browser DevTools to visualize the box model

## Instructions

1. Open `exercise.html` and `style.css`
2. Create styles that demonstrate your understanding of the box model
3. Use browser DevTools (F12) to inspect elements and see the box model diagram
4. Experiment with different spacing values
5. Build a "card" design using box model properties

## What You're Building

A page with styled "cards" that demonstrate:
- Clear understanding of margin vs padding
- Borders with different styles
- Proper spacing between elements
- Controlled dimensions

## Success Criteria

Your page should:
- [ ] Use padding to create space inside elements
- [ ] Use margin to create space between elements
- [ ] Have borders on at least 2 elements
- [ ] Show clear understanding of when to use margin vs padding
- [ ] Have consistent, readable spacing
- [ ] Include at least one "card" design with all box model properties

## Key Concepts to Remember

### The Box Model (inside out)
1. **Content** - Your text/images
2. **Padding** - Space inside, around content
3. **Border** - Line around the element
4. **Margin** - Space outside, pushes other elements away

### Syntax Examples
```css
.element {
  /* Padding (inside spacing) */
  padding: 20px;              /* All sides */
  padding: 10px 20px;         /* Vertical Horizontal */
  padding-top: 10px;          /* Individual sides */
  
  /* Border */
  border: 2px solid black;    /* Width Style Color */
  border-radius: 10px;        /* Rounded corners */
  
  /* Margin (outside spacing) */
  margin: 20px;
  margin-bottom: 30px;
  
  /* Dimensions */
  width: 300px;
  max-width: 100%;            /* Responsive */
  height: 200px;
}
```

## Common Mistakes to Avoid

- Using margin when you want padding (or vice versa!)
- Forgetting units (must write `20px` not `20`)
- Incomplete border declarations (need width, style, AND color)
- Confusing the shorthand order (Top, Right, Bottom, Left = TRouBLe)

## Using DevTools to Learn

**This is super important!**
1. Right-click any element → Inspect
2. Look for the box model diagram in DevTools
3. See the layers: content (blue), padding (green), border (yellow), margin (orange)
4. Hover over values to edit them live!

## Getting Help

Ask Copilot:
- "Should I use margin or padding to [do something]?"
- "My spacing looks wrong, what should I check?"
- "How do I create a card design with the box model?"

## Testing Your Work

1. Use DevTools to inspect your elements
2. Look at the box model diagram
3. Verify padding is inside and margin is outside
4. Check that borders appear as expected
5. Test that your "cards" have nice spacing

## Challenge Yourself

Try creating:
- A card with padding, border, and margin
- Rounded corners with border-radius
- Different borders on each side
- A perfectly centered element

## When You're Done

- Ask Copilot to "Check my work"
- Commit: `git add .` then `git commit -m "Complete Lesson 5 - Box Model"`
- Want more? Ask: "Give me a challenge"

## Resources

- [MDN: Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)
- [CSS Box Model Interactive Demo](https://www.w3schools.com/css/css_boxmodel.asp)
