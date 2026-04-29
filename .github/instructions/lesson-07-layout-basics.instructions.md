---
description: "Use when student is working on Lesson 7: Layout Basics - display property, positioning (static, relative, absolute), introduction to flexbox, creating simple layouts"
applyTo: "lessons/07-*/**"
---

# Lesson 7: Layout Basics

## Learning Objectives

Students will learn to:
- Understand the display property (block, inline, inline-block)
- Use positioning properties (static, relative, absolute, fixed)
- Understand document flow and how positioning affects it
- Create simple layouts using flexbox basics
- Use flexbox for horizontal and vertical alignment
- Build common layout patterns (header, content, footer)
- Understand when to use different layout techniques

## Key Concepts

### Display Property

**Block elements** (take full width, stack vertically):
```css
display: block; /* div, h1, p default */
```

**Inline elements** (only take needed width, flow horizontally):
```css
display: inline; /* span, a, strong default */
```

**Inline-block** (best of both):
```css
display: inline-block; /* Flows horizontally but respects width/height */
```

### Positioning

**Static** (default, normal flow):
```css
position: static;
```

**Relative** (offset from normal position):
```css
position: relative;
top: 10px;      /* Moves down 10px from where it would be */
left: 20px;     /* Moves right 20px */
```

**Absolute** (removed from flow, positioned relative to parent):
```css
position: absolute;
top: 0;
right: 0;       /* Positioned at top-right of parent */
```

**Fixed** (fixed to viewport, doesn't scroll):
```css
position: fixed;
top: 0;
left: 0;        /* Stays at top of screen */
```

### Flexbox Basics

**Container** (parent):
```css
.container {
  display: flex;
  justify-content: center;    /* Horizontal alignment */
  align-items: center;        /* Vertical alignment */
  flex-direction: row;        /* row or column */
  gap: 20px;                  /* Space between items */
}
```

**Items** (children):
```css
.item {
  flex: 1;                    /* Grow to fill space */
  flex-shrink: 0;             /* Don't shrink */
}
```

## Teaching Guidance

**Advanced concepts!** Students need to experiment to understand layout.

### Approach
- Heavy emphasis on visual experimentation
- Use browser DevTools to see layout changes in real-time
- Encourage "break it and fix it" learning
- Ask students to predict what will happen, then test
- Build understanding through problem-solving (e.g., "How would you center this?")

### When Students Get Stuck

**If elements aren't positioning correctly:**
- Ask: "What's the parent element? Is it positioned?"
- Teach: Absolute positioning needs a positioned parent (relative, absolute, or fixed)
- Show: Use DevTools to visualize positioning context

**If flexbox isn't working:**
- Ask: "Which element is the flex container? Which are the items?"
- Check: Is `display: flex` on the parent?
- Clarify: Flexbox properties split between container and items

**If layout breaks:**
- Celebrate the break! "Great, you found the limit. Now let's understand why."
- Teach debugging: Comment out properties one by one to find the issue
- Ask: "What do you think is causing this?"

## Common Mistakes

1. **Absolute positioning without positioned parent** - Will position relative to viewport
2. **Putting flex properties on wrong element** - justify-content goes on container, not item
3. **Forgetting display: flex** - Other flexbox properties won't work without it
4. **Confusing flex-direction** - Row is horizontal, column is vertical
5. **Using positioning for everything** - Often margin/padding is simpler
6. **Fixed positioning without knowing consequences** - Element stays in place when scrolling
7. **Inline elements with width/height** - Doesn't work, use inline-block or block
8. **Not understanding document flow** - Absolute/fixed elements are removed from flow

## Validation Checklist

When student asks "Check my work", verify:
- [ ] Understands difference between block, inline, inline-block
- [ ] Positioning is used appropriately (not overused)
- [ ] Absolute positioning has a positioned parent if needed
- [ ] Flexbox container has `display: flex`
- [ ] Flexbox properties are on correct elements (container vs items)
- [ ] Layout works at different screen sizes (reasonable flexibility)
- [ ] Elements aren't overlapping unintentionally
- [ ] Can explain why they chose each layout technique

## Challenge Ideas

For students who finish early:
1. "Create a navigation bar that stays at the top when you scroll (hint: position: fixed)"
2. "Use flexbox to create a three-column layout that wraps on small screens"
3. "Create a centered card using both flexbox and positioning—which is easier?"
4. "Build a 'sticky footer' that always stays at the bottom even if content is short"
5. "Research: Try using flex-wrap to create a responsive image gallery"
6. "Create a layout with a sidebar and main content area using flexbox"
7. "Experiment with z-index to layer positioned elements"

## Example Hints (graduated)

**Level 1:** "Flexbox works on a container-item model. Put `display: flex` on the parent, then use justify-content and align-items to arrange the children."

**Level 2:** "To center those elements, make their parent a flex container with `display: flex; justify-content: center; align-items: center;`"

**Level 3:** "Your parent div needs to become a flex container. Add `display: flex;` to it, then you can use justify-content to space the children."

**Level 4 (similar example):**
```css
/* Centering elements with flexbox */
.container {
  display: flex;
  justify-content: center;  /* Horizontal centering */
  align-items: center;      /* Vertical centering */
  min-height: 200px;        /* Needs height to see vertical centering */
}

/* Three-column layout */
.three-columns {
  display: flex;
  gap: 20px;
}

.column {
  flex: 1;  /* Each column takes equal space */
}
```

## Layout Debugging Strategies

**Use visual aids:**
1. Add temporary background colors to see element boundaries
2. Add temporary borders to see box dimensions
3. Use DevTools to toggle properties on/off
4. Inspect element to see computed layout values

**Common debugging questions:**
- "Is the parent a flex container?"
- "Which element are you trying to move?"
- "Is the element positioned (for top/left to work)?"
- "Are you moving the right element, or should you move its parent?"

## Positioning Context

**Critical concept:** Absolute positioning finds the nearest positioned ancestor.

Teach the pattern:
```css
/* Parent creates positioning context */
.parent {
  position: relative; /* Doesn't move, just creates context */
}

/* Child positions relative to parent */
.child {
  position: absolute;
  top: 10px;
  right: 10px;
}
```

## Flexbox Mental Model

**Container** controls overall layout:
- `justify-content`: main axis (horizontal if row, vertical if column)
- `align-items`: cross axis (vertical if row, horizontal if column)
- `flex-direction`: which way items flow
- `gap`: spacing between items

**Items** control individual behavior:
- `flex`: how much space to take
- `align-self`: override container's align-items for one item

## When to Use What

Help students develop intuition:
- **Flexbox**: Modern, powerful, great for nav bars, cards, galleries
- **Relative positioning**: Small adjustments without affecting layout
- **Absolute positioning**: Overlays, badges, decorative elements
- **Fixed positioning**: Navigation bars, back-to-top buttons
- **Grid** (future lesson): Complex two-dimensional layouts

## Encouragement Notes

- Layout is one of the hardest CSS topics—struggle is normal!
- Celebrate when layouts work, especially first centered element
- Remind them: Professional developers look up flexbox properties regularly
- Frame "breaking" layouts as valuable learning
- Point out: They're solving the same problems as professional web developers
- Emphasize: Understanding layout unlocks building any design they can imagine
- This lesson has a steep learning curve, but the payoff is huge
