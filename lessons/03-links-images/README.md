# Lesson 3: Links and Images

## Learning Objectives

In this lesson, you will learn:
- How to create hyperlinks with anchor tags
- How to add images to your page
- The difference between relative and absolute URLs
- How to write good alt text for accessibility
- How to organize files and use correct file paths

## Instructions

1. Open `exercise.html` in VS Code
2. Complete the HTML document by adding links and images
3. Create an `images` folder in this lesson directory
4. Find or download 2-3 images and save them in the `images` folder
5. Link those images in your HTML
6. Add links to your favorite websites
7. Preview your work using Live Server

## What You're Building

A personal page with:
- Links to your favorite websites
- At least 2 images with proper alt text
- A clear structure with headings and paragraphs
- All working links and images

## Success Criteria

Your page should:
- [ ] Have at least 3 working external links
- [ ] Include at least 2 images that display correctly
- [ ] Have meaningful alt text for all images
- [ ] Use proper file paths for images
- [ ] Have descriptive link text (not "click here")
- [ ] Images are in an `images` subfolder
- [ ] All links open in the browser when clicked

## Key Concepts to Remember

### Links
```html
<a href="https://example.com">Link Text</a>
```
- `href` is the destination URL
- External links need `https://`
- Link text should describe where the link goes

### Images
```html
<img src="path/to/image.jpg" alt="Description of image">
```
- `src` is the path to the image file
- `alt` describes the image (important for accessibility!)
- Images are self-closing (no </img> tag)

### File Paths
- `images/photo.jpg` - file in images subfolder
- `../photo.jpg` - file in parent folder
- `https://example.com/photo.jpg` - external image

## Setup Steps

Before you start coding:
1. Create a folder called `images` inside the `lessons/03-links-images/` folder
2. Find 2-3 images you'd like to use (photos, artwork, anything appropriate)
3. Save them in the `images` folder
4. Note the filenames exactly (including .jpg, .png, etc.)

## Common Mistakes to Avoid

- Forgetting `https://` in external links
- Wrong file paths (check spelling and folder structure!)
- Missing alt text
- Spaces in filenames (use hyphens or underscores instead)
- Trying to close img tags (they're self-closing!)
- Using "click here" as link text

## Getting Help

If you're stuck:
- Images not showing? Check: file exists, path is correct, filename matches exactly
- Links not working? Check: href has full URL with https://
- Ask Copilot: "My image isn't showing, what should I check?"
- Ask Copilot: "Check my work" when done

## Testing Your Work

1. Open in browser or Live Server
2. Do all images appear? If not, check file paths
3. Click all links—do they go to the right places?
4. Right-click → Inspect to check for errors in browser console
5. Hover over images—alt text should appear as tooltip

## When You're Done

- Ask Copilot to "Check my work"
- Commit your progress: `git add .` then `git commit -m "Complete Lesson 3"`
- Ready for CSS? Move on to Lesson 4!
- Want a challenge? Ask: "Give me a challenge"

## Resources

- [MDN: Creating Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
- [MDN: Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
- [How to write good alt text](https://supercooldesign.co.uk/blog/how-to-write-good-alt-text)
