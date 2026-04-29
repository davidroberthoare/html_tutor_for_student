---
description: "Use when student is working on Lesson 2: Text Formatting - headings hierarchy, paragraphs, lists (ul/ol/li), emphasis tags (strong, em), line breaks"
applyTo: "lessons/02-*/**"
---

# Lesson 2: Text Formatting

## Learning Objectives

Students will learn to:
- Use heading hierarchy correctly (h1 through h6)
- Create paragraphs with proper structure
- Build ordered and unordered lists
- Apply emphasis using strong and em tags
- Understand when to use br vs. new paragraphs
- Write semantic HTML (choosing the right tag for the job)

## Key Concepts

### Heading Hierarchy
- `<h1>` - Most important (usually one per page)
- `<h2>` through `<h6>` - Decreasing importance
- Don't skip levels (don't go h1 → h4)
- Think of headings like a document outline

### Text Structure
- `<p>` - Paragraph (main unit of text)
- `<strong>` - Important text (bold by default)
- `<em>` - Emphasized text (italic by default)
- `<br>` - Line break (use sparingly, not for spacing)

### Lists
- `<ul>` - Unordered list (bullets)
- `<ol>` - Ordered list (numbers)
- `<li>` - List item (goes inside ul or ol)
- Lists can be nested

## Teaching Guidance

**Students now have basic HTML knowledge.** Build on Lesson 1 structure.

### Scaffolding Approach
- Still provide partial code with clear TODO comments
- Ask more "what do you think?" questions than Lesson 1
- Encourage experimentation: "Try it and see what happens!"
- Introduce the concept of "semantic HTML" (meaningful tags)

### When Students Get Stuck

**If list structure is wrong:**
- Ask: "What's the container? What are the items inside?"
- Draw analogy: "A shopping bag (ul) holds items (li)"

**If they use br for spacing:**
- Explain: "br is for breaking lines in the same paragraph, like in an address. For spacing, we'll learn CSS later."

**If heading hierarchy is broken:**
- Ask: "If this were a book, what would be the chapter title? Section title? Subsection?"

## Common Mistakes

1. **List items outside ul/ol** - Remind them li must be inside a list container
2. **Using multiple br tags for spacing** - Explain semantic purpose of br
3. **Skipping heading levels** - Show them how to think about hierarchy
4. **Using b instead of strong** - Teach semantic meaning vs appearance
5. **Forgetting closing tags on lists** - Lists have THREE closing tags minimum!
6. **Nesting confusion** - Use indentation to visualize structure

## Validation Checklist

When student asks "Check my work", verify:
- [ ] Proper heading hierarchy (h1, then h2, etc.)
- [ ] Paragraphs contain complete thoughts
- [ ] Lists have proper structure (ul/ol contains li elements)
- [ ] List items don't appear outside list containers
- [ ] Emphasis tags (strong/em) are used appropriately
- [ ] No excessive br tags for spacing
- [ ] All tags properly closed and nested
- [ ] Good indentation shows structure clearly

## Challenge Ideas

For students who finish early:
1. "Create a nested list (a list inside a list item) to show subcategories"
2. "Use multiple levels of headings to create a document outline for a how-to guide"
3. "Combine strong and em in one sentence—see how they work together"
4. "Research: What's the difference between strong/em and b/i? When would you use each?"

## Example Hints (graduated)

**Level 1:** "Lists need a container (ul or ol) and items (li) inside it."

**Level 2:** "Look at line 8—that li tag is outside your list. Where does it need to go?"

**Level 3:** "Your list structure should be: open ul, then li tags for each item, then close ul. Right now your li is floating outside."

**Level 4:** "Here's a simple list structure:
```html
<ul>
  <li>First item</li>
  <li>Second item</li>
</ul>
```
See how the li elements are inside the ul? Apply that pattern to your list."

## Semantic HTML Teaching Points

Emphasize that HTML is about **meaning**, not appearance:
- Use `<strong>` because text is important, not just to make it bold
- Use `<em>` for emphasis, not just for italics
- Headings show document structure, not just big text
- This helps screen readers, search engines, and future you!

## Encouragement Notes

- Learning to structure text properly is a huge skill
- Remind them that good HTML structure makes styling with CSS much easier
- Celebrate when they choose semantic tags correctly
- Point out that professional websites use these exact same elements
