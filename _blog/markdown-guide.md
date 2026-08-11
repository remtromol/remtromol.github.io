---
layout: post
title: "Markdown Basics: A Quick Reference Guide for Jekyll"
date: 2026-08-05
author: "Naufal Fakhri"
excerpt: "A complete cheatsheet on writing, formatting, and adding media to .md files for blog posts and portfolio documentation."
---

Markdown (`.md`) is a lightweight text-formatting syntax that lets you write readable content without cluttering your file with raw HTML tags. When Jekyll builds your site, it automatically parses Markdown files into clean HTML.

Here is a quick reference guide on everything you can build using Markdown files.

---

## 1. Headings

Use `#` symbols before your text to create titles and section headers. 

```markdown
# Heading 1 (Main Page Title - Usually handled by Front Matter)
## Heading 2 (Main Section Breaks)
### Heading 3 (Sub-sections)
#### Heading 4 (Minor Sub-sections)
```

## 2. Text Formatting

Apply simple symbols around your words to style text:

**Bold text** for emphasis<br>
*Italic text* for subtle highlights<br>
***Bold and italic*** for extra emphasis<br>
~~Strikethrough text~~<br>
`Inline code` for short references like variables or commands<br>

## 3. well, images

you can use this format :

`![alt text](your-image-path.png)`

or this one, to prevent broken image paths when you hosted on github page:

`!["alt text"]({{ "/assets/images/posts/model-render.jpg" | relative_url }})`

it looks like this 

!["screenshot"]({{ '/image/blog/screenshot-of.webp' | relative_url }})

## 4. Lists

bullet lists:
* 3D Asset Creation
- Retopology & UV Mapping
+ PBR Texturing

numbered lists:
1. Export high-poly mesh from Blender
2. Bake maps in Substance Painter
3. Set up material shaders in-engine

checklist:

- [x]   High-poly modeling completed
- [x]   UV unwrapping finished
- [ ]   Final renders in Cycles

## 5. Blockquotes

Use the `>` character to highlight key quotes, notes or tips:

>Documenting the creation process is just as important as presenting the final render.

## 6. Code Blocks & Syntax highlighting

To display multi-line code blocks, wrap the code with triple backticks (```). You can add the language name right after the top backticks for syntax coloring:

```
{
  "assetName": "Sci-Fi Console",
  "polygonCount": 18450,
  "textureResolution": "4096x4096"
}
```

## 7. Data Tables

Create structured spec sheets or quick comparisons using pipes `|` and dashes `-`:


| Asset Name | Triangle Count | Texture Maps | Render Engine |
| :--- | :---: | :---: | ---: |
| Classic Car Chassis | 48,200 | Albedo, Normal, Roughness | Cycles |
| Sci-Fi Door | 8,500 | Albedo, Normal, Metallic | EEVEE |

## 8. Horizontal Rules

Use three dashes --- or asterisks *** on a blank line to insert a clean section divider line:

Section finished above.

---

New topic starts here.


## 9. Links

`My portfolio url is [remtromol.site](https://remtromol.site).`

My portfolio url is [remtromol.site](https://remtromol.site)