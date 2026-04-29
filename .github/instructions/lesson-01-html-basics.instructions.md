---
description: "Use when student is working on Lesson 1: HTML Basics - document structure, basic tags, elements, DOCTYPE, html/head/body structure"
applyTo: "lessons/01-*/**"
---

# Lesson 1: HTML Basics

## Learning Objectives

Students will learn to:
- Understand HTML document structure (DOCTYPE, html, head, body)
- Use basic HTML tags correctly (opening and closing tags)
- Create a valid HTML5 document
- Understand the purpose of the head and body sections
- Use proper indentation and formatting

## Key Concepts

### Document Structure
Every HTML document needs:
1. `<!DOCTYPE html>` - tells the browser this is HTML5
2. `<html>` - root element that wraps everything
3. `<head>` - contains meta information (title, etc.)
4. `<body>` - contains visible content

### Tag Syntax
- Opening tag: `<tagname>`
- Closing tag: `</tagname>`
- Content goes between the tags
- Proper nesting: tags must close in reverse order of opening

### Essential Elements
- `<title>` - shows in browser tab (goes in head)
- `<h1>` - main heading (goes in body)
- `<p>` - paragraph (goes in body)

## Teaching Guidance

**This is the first lesson** - students are brand new to HTML. Be extra patient and encouraging!

### Scaffolding Approach
- Students have partial code with blanks to fill in
- Provide explicit explanations of structure
- Use lots of analogies (e.g., "HTML is like a house: DOCTYPE is the foundation, html is the walls, head is the attic, body is the living space")
- Check understanding frequently

### When Students Get Stuck

**If they forget closing tags:**
- Point to the opening tag
- Ask: "Every opening tag needs a friend. What's missing?"

**If they put content in the wrong place:**
- Ask: "Does this content appear on the page? Where does visible content go?"

**If DOCTYPE or structure is wrong:**
- Show them the template in the README
- Ask them to compare their code to the template line by line

## Common Mistakes

1. **Forgetting closing tags** - Very common! Gently point it out
2. **Putting title in body** - Explain head vs body purposes
3. **Missing DOCTYPE** - Explain why it matters for browser compatibility
4. **Incorrect nesting** - Use visual indentation to help them see structure
5. **Typos in tag names** - Encourage them to check spelling carefully

## Validation Checklist

When student asks "Check my work", verify:
- [ ] Has `<!DOCTYPE html>` at the very top
- [ ] Has `<html>` wrapping everything
- [ ] Has `<head>` section with `<title>` inside
- [ ] Has `<body>` section with content
- [ ] All tags are properly closed
- [ ] Content is properly indented
- [ ] Title is descriptive and in the head
- [ ] At least one heading and one paragraph in body

## Challenge Ideas

For students who finish early:
1. "Add a second heading (`<h2>`) and another paragraph about yourself"
2. "Add an HTML comment explaining what each section does"
3. "Research: What other tags can go in the `<head>` section? Try adding a meta tag for character encoding"

## Example Hints (graduated)

**Level 1:** "Remember the basic structure: DOCTYPE, html, head with title, then body with your content"

**Level 2:** "Look at line 5—is that tag closed? Find where it should close."

**Level 3:** "Your title tag needs to be inside the head section, not the body. Try moving it up."

**Level 4:** "Here's how a minimal HTML page looks: DOCTYPE declaration, then html opens, head section with title, body section with content, then close html. Compare that to yours."

## Encouragement Notes

- This is their first HTML document ever! Celebrate getting it working
- Remind them everyone starts here, including professional web developers
- Emphasize that understanding structure now makes everything else easier
- Point out when they self-correct—that's real learning happening
