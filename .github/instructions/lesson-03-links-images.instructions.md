---
description: "Use when student is working on Lesson 3: Links and Images - anchor tags, href attributes, absolute vs relative URLs, img tags, alt text, file paths"
applyTo: "lessons/03-*/**"
---

# Lesson 3: Links and Images

## Learning Objectives

Students will learn to:
- Create hyperlinks using anchor tags
- Understand href attribute and URL structure
- Use relative vs absolute paths correctly
- Add images with img tags
- Write meaningful alt text for accessibility
- Understand self-closing tags
- Link to external websites and internal pages

## Key Concepts

### Links
- `<a href="URL">Link text</a>` - Anchor tag for hyperlinks
- `href` attribute specifies destination
- Link text should be descriptive (not "click here")
- External links: full URL with https://
- Internal links: relative path to other pages

### Images
- `<img src="path" alt="description">` - Image tag (self-closing)
- `src` attribute specifies image location
- `alt` attribute describes image (crucial for accessibility)
- No closing tag needed for img
- Support formats: .jpg, .png, .gif, .svg, .webp

### File Paths
- **Relative:** `images/photo.jpg` (same project)
- **Absolute:** `https://example.com/photo.jpg` (full URL)
- Go up one folder: `../images/photo.jpg`

## Teaching Guidance

**Last scaffolded lesson.** Students should be getting more comfortable with HTML.

### Scaffolding Approach
- Provide some starter code but leave more blank than Lesson 2
- Encourage independent problem-solving first, then hints
- Introduce debugging: "The image isn't showing—what could be wrong?"
- Start asking them to explain their code choices

### When Students Get Stuck

**If links don't work:**
- Ask: "What's in your href? Is it a complete URL with https://?
- Have them click the link and look at browser's address bar

**If images don't appear:**
- Ask: "Where is your image file? What's the path from your HTML file to the image?"
- Teach debugging: Check the file exists, check the path, check the filename matches exactly

**If alt text is missing or poor:**
- Ask: "If someone couldn't see this image, how would you describe it to them?"

## Common Mistakes

1. **Missing href or src attributes** - The tag is useless without them!
2. **Forgetting https:// in external links** - Link will try to load local file
3. **Wrong file paths** - Case sensitivity, typos, wrong folder structure
4. **Generic alt text** - "image" or "photo" doesn't help anyone
5. **Trying to close img tag** - It's self-closing, like `<br>`
6. **"Click here" link text** - Should describe destination instead
7. **Spaces in filenames** - Causes path issues; use hyphens or underscores

## Validation Checklist

When student asks "Check my work", verify:
- [ ] All links have href attributes with valid URLs
- [ ] External links include https://
- [ ] Link text is descriptive (not "click here")
- [ ] All images have src attributes with correct paths
- [ ] All images have meaningful alt text
- [ ] Image files actually exist in specified location
- [ ] File paths match actual folder structure
- [ ] No attempt to close img tags
- [ ] Links are clickable and go to correct destination

## Challenge Ideas

For students who finish early:
1. "Make one of your images into a clickable link (wrap img in an a tag)"
2. "Create a link that opens in a new tab (research the target attribute)"
3. "Add an image with a relative path that's in a subfolder"
4. "Research: What's the difference between .jpg and .png images? When would you use each?"
5. "Add a 'back to top' link that jumps to the top of the page (research anchor links)"

## Example Hints (graduated)

**Level 1:** "Links need two parts: the tag `<a>` and the destination `href='...'`"

**Level 2:** "Your link is missing the href attribute. After the 'a', add href='URL' before the closing >"

**Level 3:** "It should look like: `<a href='https://example.com'>Link Text</a>`. The href goes inside the opening tag."

**Level 4 (similar example):**
```html
<!-- Example link structure -->
<a href="https://github.com">Visit GitHub</a>
```

## Accessibility Teaching Points

**Alt text matters!** Teach students that:
- Screen readers read alt text to users who can't see images
- Alt text shows if image fails to load
- Good alt text describes what's important about the image
- Decorative images can have empty alt (`alt=""`)
- Example: `alt="Golden retriever puppy playing with red ball"` not `alt="dog"`

## Debugging Skills

This is a great lesson to teach debugging:
- "Image not showing? Check: Does file exist? Is filename spelled exactly right (including capitals)? Is it in the right folder?"
- "Link not working? Check: Did you include https://? Did you spell the URL correctly?"
- Use browser DevTools: Right-click → Inspect to see errors

## Encouragement Notes

- Links and images make pages come alive—this is exciting!
- Celebrate when images appear for the first time
- Remind them they're building real web pages now
- Point out that they're using the same tags as professional websites
- Debugging is a crucial skill—frame troubleshooting as learning, not failing
