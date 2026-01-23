# konnerhorton.com

Personal portfolio and blog built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

Check it out here: [konnerhorton.com](https://konnerhorton.com/)

## Prerequisites

- [Hugo](https://gohugo.io/installation/) (extended version recommended)

## Development

```bash
# Clone with submodules (for the theme)
git clone --recurse-submodules <repo-url>

# Start development server
hugo server -D

# Build for production
hugo
```

The site will be available at `http://localhost:1313/`

## Structure

```
.
├── content/
│   ├── posts/          # Blog posts
│   └── resume.md       # Resume page
├── layouts/
│   └── partials/       # Custom partials (MathJax support)
├── static/
│   ├── images/         # Images
│   ├── svg/            # SVG graphics
│   └── favicons/       # Favicon files
├── themes/
│   └── PaperMod/       # Theme (git submodule)
└── hugo.toml           # Site configuration
```

## Adding Content

### New blog post

```bash
hugo new posts/my-new-post.md
```

Or create a markdown file manually in `content/posts/` with frontmatter:

```yaml
---
title: "My Post Title"
date: 2024-01-01
math: true  # Enable MathJax for this post
---
```

## Features

- Dark/light mode toggle
- MathJax support for LaTeX equations
- Syntax highlighting for code blocks
- RSS feed
- Search (JSON index)

## Deployment

Build command: `hugo`
Output directory: `public`