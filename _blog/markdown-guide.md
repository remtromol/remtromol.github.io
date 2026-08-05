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

## 2. Text Formatting

Apply simple symbols around your words to style text:

**Bold text** for emphasis
*Italic text* for subtle highlights
***Bold and italic*** for extra emphasis
~~Strikethrough text~~
`Inline code` for short references like variables or commands

## 3. well, images

`![alt text](your-image-path.webp)`

it looks like this 

![screenshot]({{ '/image/blog/screenshot-of.webp' | relative_url }})